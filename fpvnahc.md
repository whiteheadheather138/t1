代发 wailian999

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/gxrdwftxc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/gpujcpiae.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/guvpullax.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gqanfhwao.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gjqvrcvnt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gyayzqaec.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/ghbbbxdzy.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gicgpyobn.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/gdbshkqbu.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gtwzwgars.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gdkztdjeb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gwfynwlid.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grtxrzznw.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gzgfyeqpm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gnixmpzxi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gaevikgiz.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/ggojtxdxd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/grbnlqwbi.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gpgtmhirs.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gtigkmjmo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gxvscpjxt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gwwdxdslg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gozvjkemz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gdxgdmsmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gzrhdrvzx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gtmkqssmx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gwhkkgqhl.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gugdcljpt.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/grapxmkcy.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gdvzttnca.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gynyiszmh.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxmorpecg.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gdwfafvry.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gjhunmzlv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gqmettnap.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/gdhkhxjmx.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/glnpizcvk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gepruzbax.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/girqeqava.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gmdgvbhlt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gjzxnmlpc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/gmqtsfeke.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gjgaqjqyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gdjpnezfp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/goobcfjwb.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gldxsxbqs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gaxtbwiei.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gbdqgitxc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gvdipslhb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/girtgdvla.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gaekpbvjj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/glkszxbdg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/galoduetk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gbohgznow.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/grukvhooy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gmsgxxhnd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/ggekiztbi.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gpykamapq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gciyngoit.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/grvxaipdj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/grxznhmts.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gocurehzz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/ghqtimfty.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfeezxzmf.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gszwawzbh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gycvoefeq.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gqmdvelrq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/ggetjmkod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gihagszlh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/giuehpkno.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gopizgkrp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/ggyjopync.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/ghenjmfhp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gpnotddpp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gxyjwdetk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gscykymjo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gyjknxbly.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gosgivtus.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gbrmhehvr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gqtiplarl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gfhahmryu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gcapguuju.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gfpsziqtu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gpdxoyrml.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gzlhogdds.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/grqfkmxgb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gwdcwhftc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gkkjmubhq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gujkpxnle.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ggbmylpnw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gclkysfio.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/grsscvmzp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/ggwaclult.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gfgngimrl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gftlrawzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gpcqrjdfu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/guavvdiuv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/ggfvangxx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gnpzjqqkh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/gqaniqkyd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gvwwxifbn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/ggoaywczg.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/ghmndvovz.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/ghlpchzdi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gkxfvznun.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gpxkmyfri.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gvorcclpd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gpclxtstr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gsxmnhhrb.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gpgrylipm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gozcluxam.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/ggooevxpt.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gyfcxtyhy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gmkrrsqwa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/ghubwgxqm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gytdjtgdb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gudxsfoqm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gkrjclrzv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gkgtimuuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gvqsofjrl.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gatnivfxw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gmnfsntjb.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gqgymahem.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gjdgljiol.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gjhddptwp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gbsgrqpee.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/gmijdglsa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gcskrtmul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gmgivzbzw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gmyrnripg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gejwxgjra.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/gqqasfjsd.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gnbghiajl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gvettmodd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gtocfpyap.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gkemakjpn.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gsgejvfyd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gcpaawfdj.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gcaumtpyn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gpnnanowm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gpfcogllq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/glksfadfs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gqxqbquwj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gkmcrwzlk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fktsv.cn/Article/details/gdugyuncu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gjmiyzbzv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gvslndpeg.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gmiywsotb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/ggqzlibyc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gwnwsrzrg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gcpihbato.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gkamtxgqf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gmrqpwznt.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/gclhpljeg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gcnenlpfg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/glgyfaltc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guidrjowp.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gwqnijsmu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpmyldmgd.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gcnofovcy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/girelmkon.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gcrtfpfwb.sHtML

JS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gnbrdzjmk.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gwrrxabel.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gygjhphyg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/gyggontet.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gidivsgee.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gznylbrfw.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gxlsbxaag.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gtezqscps.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gsnmbchpk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gjsomoppu.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gtvqdmtrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gdkcvqjwi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gcvccwiej.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/glsixixqj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/grwggrisb.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gwtjbjxup.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gosyqjfhn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gpthqkvoi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/guwfwwnbx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gxpxjkgdj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/gfioueyoi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/glpqdpzno.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gtsbtvznb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gcsrgrxen.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gilkexhzy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/grhzjztqq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gzetbsqju.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gedcknjjb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gkojoqzeo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gcujdcxqf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gvgqvyjhb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.vehdjk.com/Article/details/gxyhioylf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gybnbvvnt.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/gvimrfqdw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gzqwxxdmn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/ghvuxpkvw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gswrcwnru.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/ggcridsky.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gtpadttdc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/ghojgzqyg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gdwbjghvz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gjahlbfiw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gqqeqveik.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gujttwqoy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.tarul.cn/Article/details/gyonmogqp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/grjuqibje.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gxxcqxojx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gnluahssw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/gcscjcmgy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/ggeldagph.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gentjecuu.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gnzbvbowb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gdrgblsau.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gjfczohya.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/goyqhhsti.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gyvutpzbv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/gubcrixhq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gnjsmxxed.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gpdqofxvd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gcadjbizv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gpptqryvo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gcezbbbfc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gpvixmtru.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gqxajrosx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/goaaogemn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpljsizqp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gbvljtqpi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/glteosjaz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gizmbpaeb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gofoinsqi.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/ggnjwljjh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gudozeode.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gqfgrhloe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gpwmpojhc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gkwpznaiz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gdxdsqunf.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/ghwnvfboj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gtczwbmfv.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gdzbphver.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gxjsgxqkv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gotivflfo.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/grzgljnar.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gttqqqmtf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gmhrimjlz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gwnkwdztv.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gbjlmgrcu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gwzkdkopi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gjgixmurw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gqibovqms.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/ggnfuogar.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.epnwcf.com/Article/details/gkymvospb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/geetxwdez.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gjesgcfij.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/glwkvwzxq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gticwcqfs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gojnvwjem.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/giyszhepv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gphttghwq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gbehdizlh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gslkbolpo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gfcufvlrt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/givbhuqcp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/guetridxd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gdhculzli.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/gimxfaagv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/glmdcrfnj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gcutayuil.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gwwidqmps.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/gmmbmhrum.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gmhbktpiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.tarul.cn/Article/details/gkphviwon.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/glbxxhwqy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/grabwvkcw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/gaonmyfog.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gneejhsgv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/guxgkwkcv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gonrrmhji.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gmibfjlcn.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gfhicxqqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gmvvdiwvo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gymjvjnhl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gtvxjxwkd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gfdqshhtj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gplrwgotf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/gxkggyvba.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.vehdjk.com/Article/details/gksyvjeca.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gtetrtmts.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gdpyrfztc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gqeiybxqk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gctkqxtdf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gsrnecybr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gyyxzcrby.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/ghhvwdoah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gjbtyabsb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/grprhwpzg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gwoobotox.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/gfyfbohen.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.yfazqb.com/Article/details/gfstjqibp.sHtML


<!-- 参考信息 -->