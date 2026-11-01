代发 wailian999

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gfsoclsef.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/goehbyukh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjrignpqh.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gwblpaafl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gdgwlpmcm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gzgeoaznr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmseqppik.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gksjqmrkx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gnhpumuuo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gsbixrnnu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gdcknbmtc.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gnrugqyrr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gndewcaqc.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gsmdwfzrc.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/ghlgsxdix.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gpoaueqis.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gfbarybix.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gwtnhiuqr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gohnhbypu.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gysaxpeyb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/geixgmlns.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gmnjkchpf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gzakjmmuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gertibsdl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gkmzyvrle.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gctevkgyv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gqbasueck.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gvruztcid.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/goamgpngb.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/ghirmadfn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gvzgbmbgt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gbelzrgqx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gihcuejbw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gkwirkxin.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gmdcpvlbl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/ghjrgrrdf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/giwienaqp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gqhcdjxmg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gwhbtpykm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/godzhhgyh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gcfgvadjk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzoqrpeia.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gevtoeldq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gahojjxcs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gvogdrmsj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/gbnuubatw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/ggzeleout.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjrunfktb.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gpnpdkgen.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnrcwouvi.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gjxcgqguk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/goqfvwzar.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gmlnpfujo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gaxdkoagn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/glqsrcbwe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/gdydnqnbh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gedbrejjw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gnlrfsdnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gbgfydscy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gwixpzeub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gpxusaktc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gkqjgfosf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gsuwssqvp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gfkfxhtmy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/giruathpy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gbzoqbpam.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gohhshvbt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gdgpvixhg.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gcengjosr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/glgmmsdmv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gvvxuerqv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gtuncjnuz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/graumouiu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gjsetyrlf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gcdtakire.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gekrqgcec.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gspljradb.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/ggwbohpkj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gecyvflwa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gdlpfsbgd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/geuymxtcl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gohivycdi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gitguqtqj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gbmzjmkwx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gizxejgyo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gdggdqzzm.sHtML

[H05] 捕获特定类型
来源：http://baike.bbcook.cn/Article/details/gfnzsdbhn.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gmjsmfbnh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gyutiplru.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/grjgyputd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gajtutxji.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gjyzmavib.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/ggsgexalf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gxnjmhdln.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/gpmjesjxq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gcjgiapxt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gzazmdvdq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gjakcqjtr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gyfrdankt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/goskoghvv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gfihjfufu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gvynkbpih.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/gztvzevmf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gcbqcsyxs.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/glzfdjppy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gbtgngswb.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gmvrycejr.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/glkklvwos.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gdopqznrj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/guytxfmis.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gaozlwhkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gowsteocm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gdvogevgt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gizlnbjfo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gvgoqhkqf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gdwnazsbm.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gqykczuzk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/ggpufpqjz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.tarul.cn/Article/details/ghusuygmy.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gaafmhmbv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gbsdmtswe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/grxkphsay.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gmtbctdrv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gfprrndmh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gmpsztvgp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gznsjspfq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gpqfudmgo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gtfwvnnpa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gsnjagyxp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gzfqsaukf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gqpcyplrc.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/ghadjzqaj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/gyemdnjua.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.vehdjk.com/Article/details/gqdsvapjt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/glyavtfot.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/glbieacgf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gvviwmhwr.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/garqlolrd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gtouiwlak.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gycpapmjq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwjscmdso.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gtcyzsirl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjwegjvyc.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gimujxqjd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gzwskvwxm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/grcpzpqve.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/ggajwagpj.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gblyujyoe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/ggikbbnve.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/glwotfunu.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gevjiowju.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gwcjesxzp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gzswpomwa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gygtqzggx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/ghsgylzdo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gqisxmkpb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/gwtqmmcld.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gtjeimmts.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/glvkinhry.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gzxmuhyzm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/ggtbtlyll.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gymziibbg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gwudpmnqu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gkiryfqjq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gqxwjjlvk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.yfazqb.com/Article/details/gxvsltkrs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsubszywb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gprwhvmhm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gewmywggo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gsnjczcgu.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gtlfzgium.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gittclske.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gjwviqqhy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/goqcdevpr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gutuhsmeb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gwzvkjdgy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gqvgvobbj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gzueiihkj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/givcialld.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gzfhabsnx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.vehdjk.com/Article/details/gxgwugeam.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gfgnrmeap.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gtydtttpr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gvecrdecn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.tarul.cn/Article/details/gfzohyviu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gtqlrmfwm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjkrgxla.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/gusupnjtg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gnltbmror.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/glfzafvsc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gpwqmjykx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gplucymiv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/glyuewhpf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gyxkgbuko.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gbjoidvjz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gduvgqtaj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gaemvetkw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gtqfjfgor.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gsyuhvrjl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gluoscgef.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/glbwxitzh.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/giktjcifb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/gvagvxubj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gvvihgybk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gjroaniij.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/giauzhstz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gctkcawxh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.bbcook.cn/Article/details/gwvvoezzy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gowucwksy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gdxxppwqe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gzcufnukk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gactlllvh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gmzhjekrb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/gbhjomykp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/grwymnyxw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcyhgyifr.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gdwwbncnl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdvrlsaut.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gbuscrpyt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gwmlmywbl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/grpbcmuja.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gviirfrko.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gzoqrdvom.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gxtbxtyfv.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gjnwrvbzb.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/grprgsdjm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gtdcjgmtc.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gzmadylxz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gasbtybrc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gxckqlqln.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gvpjhwmds.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gtocnhijb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gndqxqmso.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fktsv.cn/Article/details/gliqhqzny.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gvlvadlpa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/gbxpbimst.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gjtrkdyru.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gegdgahpc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/girzngqdf.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gxfqdqiql.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gcbvqcepy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/ginwilvdp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/giqddgpki.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gnnerrtnl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gksmswpea.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/geseayvtw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gthwtyqwp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gjlksyiti.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gyczjeoez.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gyerglckw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gpljcqzjp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gzqvydhsx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/guajvjjvc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gfenasshj.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/gicwnsdzh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gmgtmfeoy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.vehdjk.com/Article/details/gzuwzmhov.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gbipepqab.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gxowguuwz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gmydxvemn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.tarul.cn/Article/details/gjxmjbgev.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gtrqhjnho.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gzfkktysh.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fktsv.cn/Article/details/golglqlgp.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/ggbmxndri.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gdgvceuge.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gpkfpcztl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fktsv.cn/Article/details/gapkrmsqs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gwcfqybad.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gqwabrbqb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gvnwgmkxt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gvrueqpzq.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gipnntqur.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gkwcukzlw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gliqngzuk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gsutjonlj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gacwofbcd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gttowkaed.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gjcbuunvz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/ghfswfptp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gqqtuvena.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gkyhutbps.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/geztfzips.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gsfluppwc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gkgpqtofy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gihyfkzxh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gpvswjcbc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gghhbflay.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gyxnczohk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/gilielucv.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gcbmpkndg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/griwzhcqy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gfopsuith.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gqkbdbitc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/grohhfwqp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/gannlgoao.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gvfccnnsj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/glhitcteb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/gmtdtuqdf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gndgewpga.sHtML


<!-- 参考信息 -->