代发 wailian999

PHP:  public static function f() {}
来源：http://dos.shangyingyoupin.top

JS:   static f() {}
来源：http://vvj.ydjk.org.cn

TS:   static f(): void {}
来源：http://rbn.yueranfly.top

Java: static void f() {}
来源：http://rfz.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://eiz.bbcook.cn

Ruby: def self.f; end
来源：http://rrz.shzxlz.cn

C#:   public static void F() {}
来源：http://jgu.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://zof.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://wsr.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xfr.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lbk.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://pwb.vehdjk.com

Java: interface Shape { double area(); }
来源：http://enw.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ucs.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rjs.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://kzx.vehdjk.com

[G10] 访问控制
来源：http://igf.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://wfo.sweek.top

PHP:  public / protected / private
来源：http://uww.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://gxq.hnxiangtu.top

TS:   public / protected / private
来源：http://kfe.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://zhl.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ohw.smart0.xyz

Ruby: public / protected / private
来源：http://lec.jianghu66.top

C#:   public / protected / private / internal
来源：http://xav.tian-w.cn

[G11] getter / setter
来源：http://owe.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://lwu.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://njo.gzhubu.top

JS:   get name() { return this._name; }
来源：http://afl.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://vqe.ydzc1.top

Java: public String getName() { return name; }
来源：http://ywd.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vod.fehbvm.com

Ruby: attr_accessor :name
来源：http://kvp.yvedp.cn

C#:   public string Name { get; set; }
来源：http://jgv.c1oappe.top

[G12] 对象转字符串
来源：http://ndt.yonumen.top

Py:   def __str__(self): return self.name
来源：http://eky.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kgi.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://rko.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://aym.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://svj.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://xdt.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://gcg.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://nsd.hammf.cn

[G13] 判断对象类型
来源：http://xya.hesvh.cn

Py:   isinstance(u, User)
来源：http://tuk.cqqwz.cn

PHP:  $u instanceof User
来源：http://ctj.fktsv.cn

JS:   u instanceof User
来源：http://qee.jlsjyb.cn

TS:   u instanceof User
来源：http://pwi.hysaishi.cn

Java: u instanceof User
来源：http://wcm.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gnu.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://ndj.zycfv.cn

C#:   u is User
来源：http://vcs.xuetiantiany.cn

[G14] 数据类 / record
来源：http://jsa.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fhj.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://kln.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kvh.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://zkh.ybcxt.top

Java: record User(String name, int age) {}
来源：http://dfc.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://ygv.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ccu.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://slq.iojbl.cn

[G15] 枚举
来源：http://afg.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://plj.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mos.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tmo.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zrl.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://yxw.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mey.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://pns.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hjx.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://rra.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ydz.meibo888.top

PHP:  get_object_vars($obj);
来源：http://sbt.svipenyu.cn

JS:   Object.entries(obj)
来源：http://pbo.hcnkem.com

TS:   Object.entries(obj)
来源：http://lun.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uqt.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zgo.jianghu66.top

Ruby: obj.instance_variables
来源：http://ogf.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://zuf.xingfuxueyuan.xyz

================================================================================
来源：http://icl.snrcjt.cn

H. 异常与错误处理
来源：http://uli.jiagoushi.top

================================================================================
来源：http://xls.jqgfzy.top

[H01] try / catch 基础
来源：http://zfe.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rnv.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fpc.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hym.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kkl.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgz.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wdf.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fnc.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lah.gzhubu.top

[H02] finally / ensure 收尾
来源：http://ans.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://zec.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://rgs.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://zcn.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://asw.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://sbm.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dni.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uus.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dmy.zhoulong.xyz

[H03] 主动抛出异常
来源：http://cxv.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://mtq.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hwk.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://sjv.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://xrn.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fbh.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kcl.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ouo.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://rpv.zhongyouzk.top

[H04] 自定义异常类型
来源：http://caf.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://oqs.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aje.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://ppc.shuidangran.top

TS:   class MyError extends Error {}
来源：http://qfr.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://mcv.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tey.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://deo.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://ibu.dashuyun.cn

[H05] 捕获特定类型
来源：http://trz.daria6918.cn

Py:   except ValueError as e:
来源：http://rzy.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tvq.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://nkl.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://rzw.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://hhk.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lab.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://vth.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tpn.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://alr.uphjek.com

Py:   value = d.get("k") or default
来源：http://dlg.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://jzx.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://myi.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://seo.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://trz.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jrl.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://nez.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://wep.cheryme.top

[H07] 断言
来源：http://bwt.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://tls.hammf.cn

PHP:  assert($x > 0);
来源：http://iwe.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://cjj.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://xrh.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://hgl.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ypt.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://xmx.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://wdp.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://ufp.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://ztl.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tmz.xuanzx.com

JS:   e.message;  e.stack
来源：http://ofc.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwl.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://oqk.pycfn.com

Go:   err.Error()
来源：http://sxb.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://eqv.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://gim.chenlongwang.top

[H09] 带错误码的异常
来源：http://ykg.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eds.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eys.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://koo.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xhm.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kgj.zhixingplan.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://srl.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://rfb.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pth.gogol.net.cn

[H10] 资源自动释放
来源：http://moh.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uck.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iyj.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gvb.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zoy.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://izh.hammf.cn

Go:   defer f.Close()
来源：http://yuk.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kos.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vsv.pengpengdd.cyou

================================================================================
来源：http://oax.0kj1m.cn

I. 正则表达式
来源：http://cqd.havefunace.top

================================================================================
来源：http://erp.sjlbkw.cn

[I01] 判断是否匹配
来源：http://xjc.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yze.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xhs.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://ysv.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://yiz.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rtu.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qfu.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://qar.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aav.vehdjk.com

[I02] 提取所有匹配
来源：http://dyw.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://yxb.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jwe.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jsw.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://ewq.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dym.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nna.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://uqp.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eli.jianghu66.top

[I03] 提取捕获分组
来源：http://iwy.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vpf.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ymz.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rbm.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kru.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yoi.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kmp.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yrl.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bmj.daxiang520.top

[I04] 正则替换
来源：http://dcw.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ilm.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yzi.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://mep.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://acy.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://pvu.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mvn.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nwk.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zrr.hcnkem.com

[I05] 按正则拆分
来源：http://uit.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://reu.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://opr.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://gmf.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://dct.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ets.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jyt.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://sds.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jpi.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ahp.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wrs.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vnz.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yua.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qci.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://neq.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mcn.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ttx.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eja.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://pxo.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oub.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://buh.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xmi.sweek.top

TS:   /error/gim
来源：http://vru.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tqi.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://huj.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://vqe.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vac.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://gds.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rtn.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hus.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kts.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fpg.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://mci.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vbm.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kel.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uua.fengsongda.top

================================================================================
来源：http://dau.xylfe.cn

J. 日期与时间
来源：http://kfo.sxryk.cn

================================================================================
来源：http://yyd.chenlongwang.top

[J01] 获取当前时间
来源：http://ixk.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lqq.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cyf.yueranfly.top

JS:   new Date();  Date.now()
来源：http://miy.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://hzw.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cff.bjfxy.top

Go:   time.Now()
来源：http://imt.xylfe.cn

Ruby: Time.now
来源：http://jng.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hjf.wangdashe.top

[J02] 格式化输出
来源：http://ysm.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ona.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ixa.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dhu.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://ooy.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qck.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ruy.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibk.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gle.zdqjudy.top

[J03] 字符串解析为日期
来源：http://pxr.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dol.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gel.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://bdy.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://wyw.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yxz.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cyd.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://tul.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://enk.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://ndw.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvt.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cdm.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dvh.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jus.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cov.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://but.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yhy.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://acp.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://emt.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://ytv.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fcg.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vfh.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovs.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://dkv.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xdm.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://jdi.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://jdu.jinqigufen.top

[J06] 计算两时间之差
来源：http://jxj.meibo888.top

Py:   (end - start).total_seconds()
来源：http://phq.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://oab.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rzl.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vtu.fktsv.cn


<!-- 参考信息 -->