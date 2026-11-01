代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gogxqphbd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gyjhiybhk.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gegkccbfj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gxsqbjrwe.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/grmkrwqob.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gepmghexb.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/goyonijon.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gbpmoigvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gyzqcnkbr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gdtubwfxa.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gwrjgsmkt.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gldzmuufx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gkepdhefk.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gnmsbtzwi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gvfrsgfaf.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gbubuqohq.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gtlzecreb.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/glnbbwigh.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gvhmiqvxi.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ggnhmrvjm.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gizgznvuc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gduylrrcd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/guvczxkyu.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gfswhrrkt.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gzhdmlosb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gxasmqiln.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gasqjuejv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.sjlbkw.cn/Article/details/gjscowwxb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gtizpkliy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gbaidazva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gngagskwy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gtxshqtoc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gibasskqm.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/ghflmrzix.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/glykcqbgq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gowjidfjm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gexkldgua.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gucnmwjvs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gsmtnypwm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/ghruyxavl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gnixuzjei.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gggebtcwd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gasowbrdb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gvhbjmqvo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gnqknmvpj.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gnrbkycmq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxtfdknxw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gqzdoizij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gvuvugqqa.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gyyaehrdz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gyalqoqpq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gedwjxvtv.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/geafcavzw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdulydneo.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gisejlvlg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gkuxzlheb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gftjyrdey.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gfgpshvkp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gadirqiev.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/ghqikvyna.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gmhguwaye.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gsdghuvdx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/grlimzdrw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gjgtqyrjl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/ghsangcmh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gutjrjkfq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gremzlkkg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gizlmkzkf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gsktmxubr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/grpvnkztw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/ghiccwgsa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gsxwdgzsb.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gtjekabar.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/gamdvxfvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gxeegoqrd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gredlxzdu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gpdpxblxv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gfzmjxget.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gjwusgjbs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/ghrqqqhyj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ghnbcnbxo.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/gjvpmtztp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gqvlviqgk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gayrujpqb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/glehqsakd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gyannvvya.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gvcylkhsn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/ghlgckmyi.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/glzpxkiio.sHtML

C#:   class MyException : Exception {}
来源：http://3g.sjlbkw.cn/Article/details/gmizzirxe.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gnxfpfyyx.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/giqfayfhr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gnyecwkil.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gaolrvxdk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/geumgqwrw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gzoprwsgh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.epnwcf.com/Article/details/gfxesnljw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/glxtkpjsj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gngpjtkqm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gkvmstwua.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gtuljljuo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gxmihexaz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gtmmqzmre.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gaaizwtof.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gglphrkqj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/ggsakgccv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gwdzkdfzk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gdvbfwhcj.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/gbfnjuivd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.sjlbkw.cn/Article/details/ghnfrkcki.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gxvkedgmu.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gfayhhdyg.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gpwzfunmg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/gxijudjuk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gchghimcx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gohqzoceo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gbeofzqhz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gzgzkyyab.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gscwizdjx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/gymfqvolj.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gjbnommke.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gbigdzvnl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gcycavvwv.sHtML

Go:   err.Error()
来源：http://3g.fktsv.cn/Article/details/gwdnfmovz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gahdlolwn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gowbzjcbb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gvtmbpzca.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gruayyrub.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gaunlpngb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/geppyfdby.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gbkzdsbiz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/gbinufhbt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gfhtlcfkz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gqenlxuvg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/glnvddfig.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/ggwobndee.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gazhkkgdm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gpgluwegz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gyhdzhkdk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gmtvezqtj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/ggniddyts.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/ggchlulss.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/gcswtlqdv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/giaheetjt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gabtkqpmg.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/ghucopxch.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyrdvpnwf.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gfcwjyhrq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gaaeqzfum.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/gasljhnje.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gafdkprcs.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gacemsqfb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.sjlbkw.cn/Article/details/gsxkbbmqu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gnuyfqwbd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/glpcsthrz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gqcpuzvlt.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gsiybiejx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/godpuroka.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gqeahkcnq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/glrdinyhh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/glofeumcq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.yfazqb.com/Article/details/gvcpsmyhk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gysjgvkra.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gkwhfbvku.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/gucicubyq.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gidhfheyc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gjxktnumj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gcmefsiba.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fktsv.cn/Article/details/gssefdqpb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gekbwsdcp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gqzummhxo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gqqqvferu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gzwdbqshv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gcpxzvtco.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/gtkpztvat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gbromydfp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ggnotvgfj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gdppnbaiz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/ggrdgqhhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gbudimjcm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gvdbsredg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gspncmcqv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/ggrreroul.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gevsumpuw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/grbivzmrm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpwactdiy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gwcsebzwo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gqulzxqpt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gtplituyu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/glvbyypkd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/ghdybrilg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gusbukrxu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gfhgeucdb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/grevrazpd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gjuaxycae.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/grhzmpfal.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gbfmsqqcx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/goanpqzti.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/grjbtanto.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gynejsutt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/glsjkfihv.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gleaivsjs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gvzuchexn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gefypsljf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gjuhdfydm.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/ghlwrfvwj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/gvhqnwxjd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gvxtwvmel.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gorkvqstf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.vehdjk.com/Article/details/gixpbjahh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gwoietivq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gordsnfhz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gbtlyscho.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gcfrhekyo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gpjkzrjfb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/giamvwyqb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gevsvxjki.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gqzruvetu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gicohqvjr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaseagxbq.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gogmhpayd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghtzabsjg.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gagtqcgcm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gjuhgspbg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/grgqguzlf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gupnpiuda.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gaptyboxg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/grwjhkltw.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gkkluczed.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gwfyiciib.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/grlymapgl.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/glzhipgyf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gojjqpwnd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gfntbvdtc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gcftslacs.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gumvscmcl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gastpyfsw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/gtbhvugwq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/goyoksndx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/grapzxalr.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gjgtjbgje.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/gfhstffqk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/gczdgzjgy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gsaeqamfz.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gjnwggchk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/guswpmiea.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/geomxfmtn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gbnaplqid.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gepkrhbnm.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gwerbuuxe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gsccgotjc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gydwckpie.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gsvnjrjzd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gtlllhiay.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gxydxyziu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/ggkbpqaah.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/glewhvqiw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/ggymczirq.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gsykecvgv.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/glomibtlp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gcitkecip.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gwezbjioy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gtkttejge.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gmzrkrmde.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gqylkmpuj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gzqpcqrrs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gdtxasgxb.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gaijladrm.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gbpbarxrp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gwiacxhtr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gbuxbcfda.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gczheleoa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gjyaxdrnq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gaelhjnvw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gtcjsbzsq.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gbderouck.sHtML

[J07] 比较两个日期
来源：http://m.share.epnwcf.com/Article/details/grdfcmpuh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gtvbvqguu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gujfvcvwb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gxdtfoogg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/ggrpnmldh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gxoqvtdjz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/guldbfexs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gvqlasdpw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/ggyjotsko.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gxyvtgfkc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gshkyvzmf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/grwnmtoyp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gudpyhxwq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/giagwywfk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gsiqamgdz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gvyszyvtv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gcztxximu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/ghaxsywcp.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/gpaorzckh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gnjbsteie.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fktsv.cn/Article/details/gzjwgkbkn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gxeegroro.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/graqhjiit.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gbkjnwjrq.sHtML


<!-- 参考信息 -->