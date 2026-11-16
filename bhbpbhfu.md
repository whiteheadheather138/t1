代发 wailian999

PHP:  public static function f() {}
来源：http://nzl.316326.xyz

JS:   static f() {}
来源：http://ksn.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://duu.cucudq.cn

Java: static void f() {}
来源：http://wfp.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://onv.zhengqikj.top

Ruby: def self.f; end
来源：http://aee.tanke756.top

C#:   public static void F() {}
来源：http://nbx.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://rkq.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://cab.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://pbu.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://fkp.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://hwl.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://sps.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://yjz.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rbn.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://gqv.52xcode.cn

[G10] 访问控制
来源：http://gei.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://gwa.jqgufenzy.top

PHP:  public / protected / private
来源：http://kli.bbcook.cn

JS:   #private 字段；其余公开
来源：http://wjk.tanke756.top

TS:   public / protected / private
来源：http://jyo.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://buy.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vid.jinqigufen.top

Ruby: public / protected / private
来源：http://rtg.ppjwa.cn

C#:   public / protected / private / internal
来源：http://ojj.gotoacloud.top

[G11] getter / setter
来源：http://rci.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://cts.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rsu.ybcxt.top

JS:   get name() { return this._name; }
来源：http://job.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://lsr.gogol.net.cn

Java: public String getName() { return name; }
来源：http://fpj.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dec.ppjwa.cn

Ruby: attr_accessor :name
来源：http://drg.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://ind.havefunace.top

[G12] 对象转字符串
来源：http://pjo.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://srj.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://szp.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://sch.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://bvv.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://qja.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://but.nwbrower.top

Ruby: def to_s; @name; end
来源：http://mew.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://umh.vehdjk.com

[G13] 判断对象类型
来源：http://jco.yuxming.cn

Py:   isinstance(u, User)
来源：http://grv.hfpthk.cn

PHP:  $u instanceof User
来源：http://avb.snrcjt.cn

JS:   u instanceof User
来源：http://zhg.hesvh.cn

TS:   u instanceof User
来源：http://tle.hywenlv.cn

Java: u instanceof User
来源：http://tby.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zxe.jianghu66.top

Ruby: u.is_a?(User)
来源：http://vmm.shangyingyoupin.top

C#:   u is User
来源：http://alf.guannengcc.top

[G14] 数据类 / record
来源：http://rww.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zdu.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://dej.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://qok.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://nmo.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://qra.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://hwt.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gso.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://vrv.shangyingyoupin.top

[G15] 枚举
来源：http://gdw.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jev.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://jac.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://edi.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zch.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://fkp.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pkd.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://imb.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpt.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://dhc.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jig.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://fnp.redwolf501.top

JS:   Object.entries(obj)
来源：http://pif.cucudq.cn

TS:   Object.entries(obj)
来源：http://rhy.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xzh.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rkd.yuxming.cn

Ruby: obj.instance_variables
来源：http://adt.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://yez.fktsv.cn

================================================================================
来源：http://vzj.chenzaomai.com

H. 异常与错误处理
来源：http://jbb.snrcjt.cn

================================================================================
来源：http://ugm.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://dhx.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dfy.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jlt.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://naw.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rbi.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jlj.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://let.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fxx.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vqm.wangdashe.top

[H02] finally / ensure 收尾
来源：http://iga.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ttd.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vuu.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ido.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ewl.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://uje.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fad.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://ida.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvt.gogol.net.cn

[H03] 主动抛出异常
来源：http://dda.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://ltl.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zye.pycfn.com

JS:   throw new Error("错误信息");
来源：http://lyn.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://fce.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mli.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wex.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://aoa.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ysy.cashguo.top

[H04] 自定义异常类型
来源：http://fbr.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://xmo.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://wei.yj20258.top

JS:   class MyError extends Error {}
来源：http://tim.cucudq.cn

TS:   class MyError extends Error {}
来源：http://jra.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://xuu.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhh.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://eys.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://ijo.ydzc1.top

[H05] 捕获特定类型
来源：http://gpb.9152youxi.cn

Py:   except ValueError as e:
来源：http://ptm.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://isx.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://yok.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://seq.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://hxy.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xvq.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://dea.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://okb.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://rxv.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://pio.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://qlr.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://lgg.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://vta.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wfy.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lrf.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://qsn.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://dis.yonumen.top

[H07] 断言
来源：http://mov.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://bkg.ivvv.top

PHP:  assert($x > 0);
来源：http://jji.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://zsp.iojbl.cn

TS:   console.assert(x > 0);
来源：http://qth.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://giq.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://krz.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://itl.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://fwl.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://fyl.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://yim.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xhe.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://gej.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ilv.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pfx.guowangkeji.top

Go:   err.Error()
来源：http://eyw.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://sia.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://qog.meibo888.top

[H09] 带错误码的异常
来源：http://sod.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qsf.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://szm.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oci.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hrc.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zjh.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rny.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://qir.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zkz.ctjpmb.com

[H10] 资源自动释放
来源：http://ubk.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tzm.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mgc.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blk.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lcl.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sfo.yuxming.cn

Go:   defer f.Close()
来源：http://kkb.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qxb.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ejq.hfpthk.cn

================================================================================
来源：http://ikp.jinghuilouyu.cn

I. 正则表达式
来源：http://odh.cashguo.top

================================================================================
来源：http://aly.zhixingplan.top

[I01] 判断是否匹配
来源：http://tdu.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eqq.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://amq.fktsv.cn

JS:   /\d+/.test(s)
来源：http://kxd.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://kat.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bpc.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lky.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://lph.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://csj.guowangkeji.top

[I02] 提取所有匹配
来源：http://hyv.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://wgc.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://flf.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mud.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://zzs.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gsw.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mdq.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://uky.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://myc.fzhhl.top

[I03] 提取捕获分组
来源：http://mhh.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zxy.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wkx.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eow.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cyh.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tyg.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gxm.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dhq.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mdl.kuanghao11.cn

[I04] 正则替换
来源：http://cav.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://buk.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dzv.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://ypt.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tlj.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://rdf.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mnz.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://otk.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vcl.jlsjyb.cn

[I05] 按正则拆分
来源：http://fyp.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gfz.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dyz.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://yoa.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://mrk.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://sis.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brq.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qpc.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fjd.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jjr.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wnf.ydjk.org.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vut.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vdo.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lqd.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jbj.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sqo.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sib.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yzv.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://kqk.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tqb.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dnp.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xsr.9152youxi.cn

TS:   /error/gim
来源：http://bwh.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cht.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bhf.uphjek.com

Ruby: s.scan(/error/i)
来源：http://zdd.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yvr.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://yxv.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rnh.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://afh.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyn.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uqw.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://duu.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ksi.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tfb.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://stp.yj202588.top

================================================================================
来源：http://lsc.havefunace.top

J. 日期与时间
来源：http://lbc.ywan-chungtsiang.top

================================================================================
来源：http://guj.ppjwa.cn

[J01] 获取当前时间
来源：http://avd.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://unx.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oiy.fzhhl.top

JS:   new Date();  Date.now()
来源：http://hoq.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://jbj.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fnb.dianchejie.cn

Go:   time.Now()
来源：http://aml.gogol.net.cn

Ruby: Time.now
来源：http://wmy.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgy.birdmap.top

[J02] 格式化输出
来源：http://mde.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://osj.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jpo.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bna.xylfe.cn

TS:   d.toISOString()
来源：http://bdl.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qob.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jij.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jyz.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uru.sxryk.cn

[J03] 字符串解析为日期
来源：http://gbi.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cei.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mya.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://ohl.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://esm.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zli.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://quy.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://tsu.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://luy.yvedp.cn

[J04] 时间戳与日期互转
来源：http://fxi.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ewz.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://koi.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://klu.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cea.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sis.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nfn.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvk.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eth.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://smd.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://org.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zwy.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://brw.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://udy.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://lms.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ora.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://ewr.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rkd.yuxming.cn

[J06] 计算两时间之差
来源：http://zlr.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://uls.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://zym.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qay.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wiv.shuidangran.top


<!-- 参考信息 -->