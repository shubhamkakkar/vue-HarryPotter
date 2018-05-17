<style scoped>
    
</style>

<template>
    <div>
        <div class="container my-5 py-5 border" style="max-width : 1110px" id="author">
            <u> <h1 class="card-title">
                    {{ bio.PenName }}
                </h1>
               </u>
            <div class="card border-0">
    
                <div class="row">
                    <div class="col-md-6">
                        <div class=" card-text" style="margin-top : 20%" >
                            <ul class="text-center" style="list-style-type: none; " v-for=" (key, value) in bio">
                                <li style="font-size : 30px">
                                    <span style="text-decoration:underline" class="font-weight-bold"> {{ value }}  </span>
                                    :
                                    <span style="font-style:italic">{{ key }}</span> 
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="card-img">
                            <img src="img/jk.jpg" class="img-fluid float-left" style="border-radius : 20px" alt="jk rowling">
                        </div>
                    </div>
                </div>
                <div class="card-body">
                    <div class="container">
                        <div class="row">
                            <div class="col-md-4">
                                <div class="card border border-danger border-right-0" style="overflow-y : scroll; max-height : 20vw">
                                    <div class="card-title text-center font-weight-bold p-2 m-auto" style="font-size : 25px; text-decoration: underline">
                                        About
                                    </div>
                                    <div class="card-body text-justify">
                                        J.K. Rowling, is a British author and screenwriter best known for her seven-book Harry Potter children's book series. J.K. Rowling was living in Edinburgh, Scotland, and struggling to get by as a single mom before her first book, Harry Potter and the
                                        Sorcerer's Stone, was published. The children's fantasy novel became an international hit and Rowling became an international literary sensation in 1999 when the first three installments of Harry Potter took over the
                                        top three slots of The New York Times best-seller list after achieving similar success in her native United Kingdom. The series has sold more than 450 million copies and was adapted into a blockbuster film franchise.
                                        Rowling published the novel The Casual Vacancy in 2012, followed by the crime novel Cuckoo Calling under the pen name Robert Galbraith in 2013. In 2016, she released a play, Harry Potter and the Cursed Child, and a
                                        movie, Fantastic Beasts and Where to Find Them.
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-4">
                                <div class="card border border-danger border-right-0" style="overflow-y : scroll; max-height : 20vw">
                                    <div class="card-title text-center font-weight-bold p-2 m-auto" style="font-size : 25px; text-decoration: underline">
                                        Net Worth
                                    </div>
                                    <div class="card-body text-justify">
                                        According to The Sunday Times 2017 Rich List, J.K. Rowling’s net worth is £650 million (about $850 million) — making her wealthier than even Queen Elizabeth II. Forbes put her wealth at $650 million in 2017, in large part due to the 450 million copies
                                        of Harry Potter sold to-date and the subsequent movie franchise that has grossed $7.7 billion. (Her worth would've been more in Forbes if it were not for the $150 million she has donated to various charities.) In the
                                        first half of 2017, Rowling took home an estimated $95 million thanks to her new play, Harry Potter and the Cursed Child, and movie, Fantastic Beasts and Where to Find Them.
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-4">
                                <div class="card border border-danger border-right-0" style="overflow-y : scroll; max-height : 20vw">
                                    <div class="card-title text-center font-weight-bold p-2 m-auto" style="font-size : 25px; text-decoration: underline">
                                        Husband And Children
                                    </div>
                                    <div class="card-body text-justify">
                                        On December 26, 2001, J.K. Rowling married anesthetist Dr. Neil Murray at the couple's home in Scotland. They have two children together, David (born in 2003) and Mackenzie (born in 2005). Rowling has one child, Jessica (born 1993), from her previous
                                        marriage.
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                bio: {
                    Name: 'Joanne Rowling',
                    PenName: ' J.K. Rowling',
                    Birthday: 'July 31, 1965'
                }
            }
        } //data
    } //export
</script>
