代发 wailian999

JS:   super.greet();
来源：http://apq.shanyushiyangkeji.top

TS:   super.greet();
来源：http://rlc.hysaishi.cn

Java: super.greet();
来源：http://alf.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qpg.52xcode.cn

Ruby: super
来源：http://iop.jianghu66.top

C#:   base.Greet();
来源：http://unm.hesvh.cn

[G08] 静态方法与属性
来源：http://wgo.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jma.sysykeji.top

PHP:  public static function f() {}
来源：http://pef.yangfankeji.com

JS:   static f() {}
来源：http://gom.tianlin.xyz

TS:   static f(): void {}
来源：http://fyl.jqgufenzy.top

Java: static void f() {}
来源：http://bay.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ooj.chenzaomai.com

Ruby: def self.f; end
来源：http://huy.cashguo.top

C#:   public static void F() {}
来源：http://eos.zycfv.cn

[G09] 接口 / 抽象类
来源：http://yvk.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gyx.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fyh.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qac.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://rjo.smart0.xyz

Java: interface Shape { double area(); }
来源：http://mun.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://dcn.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tpv.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://qor.smart0.xyz

[G10] 访问控制
来源：http://dnw.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://ncb.yj20258888.top

PHP:  public / protected / private
来源：http://vzd.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://viy.uphjek.com

TS:   public / protected / private
来源：http://yae.316326.xyz

Java: public / protected / private / 默认包级
来源：http://piq.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xcv.hysaishi.cn

Ruby: public / protected / private
来源：http://pbu.cqqwz.cn

C#:   public / protected / private / internal
来源：http://iev.zdbjq.cn

[G11] getter / setter
来源：http://zus.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://smp.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gxr.tian-w.cn

JS:   get name() { return this._name; }
来源：http://umj.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://bgo.yuanzhike.top

Java: public String getName() { return name; }
来源：http://wra.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://efp.yj20258.top

Ruby: attr_accessor :name
来源：http://dyb.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://klm.yangfankeji.com

[G12] 对象转字符串
来源：http://qtw.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://koy.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aug.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://kht.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://tug.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://gfi.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://tjf.jianghu66.top

Ruby: def to_s; @name; end
来源：http://kom.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://ihk.zhoulong.xyz

[G13] 判断对象类型
来源：http://yob.zycfv.cn

Py:   isinstance(u, User)
来源：http://zsn.ybcxt.top

PHP:  $u instanceof User
来源：http://nbu.daria6918.cn

JS:   u instanceof User
来源：http://wvs.ctjpmb.com

TS:   u instanceof User
来源：http://rig.nanxuanxn.top

Java: u instanceof User
来源：http://nfx.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zfr.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://mbv.sjlbkw.cn

C#:   u is User
来源：http://bin.tian-w.cn

[G14] 数据类 / record
来源：http://bym.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iiy.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://qht.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://qpl.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://wqn.sweek.top

Java: record User(String name, int age) {}
来源：http://hny.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://sbz.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kcb.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://uqg.sweek.top

[G15] 枚举
来源：http://kcj.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xbz.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://scu.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fqg.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kcx.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://ozw.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uab.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://duw.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://epi.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://ihz.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjb.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://rnv.yongpay.top

JS:   Object.entries(obj)
来源：http://icc.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://nqk.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nek.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ovs.ppjwa.cn

Ruby: obj.instance_variables
来源：http://dha.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://gti.meibo888.top

================================================================================
来源：http://rsc.gotoacloud.top

H. 异常与错误处理
来源：http://loh.birdmap.top

================================================================================
来源：http://drz.jianghu66.top

[H01] try / catch 基础
来源：http://vng.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://isw.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rmn.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cit.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qpu.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yzh.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cwj.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tfy.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ezy.sxryk.cn

[H02] finally / ensure 收尾
来源：http://gtn.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://fzm.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gdr.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cqe.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://esh.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://yvy.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nsk.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yuc.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibu.hesvh.cn

[H03] 主动抛出异常
来源：http://kio.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://ieh.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kuo.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://tfp.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://qyz.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nic.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pox.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cwx.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://esz.yj20258.top

[H04] 自定义异常类型
来源：http://fez.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://rgz.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://hwt.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://kxd.yvedp.cn

TS:   class MyError extends Error {}
来源：http://ptd.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://wgc.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nky.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://ugl.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://wnn.aibaodan.cn

[H05] 捕获特定类型
来源：http://cgy.hysaishi.cn

Py:   except ValueError as e:
来源：http://slr.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gzl.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://xti.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://dxi.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://evt.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qyw.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://bbd.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wzl.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://bkb.hcnkem.com

Py:   value = d.get("k") or default
来源：http://izc.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://uze.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ynw.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://hjz.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vnv.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://amh.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://bai.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://ruc.ehwqpu.com

[H07] 断言
来源：http://gvv.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://nji.yongpay.top

PHP:  assert($x > 0);
来源：http://zjl.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://wmd.52xcode.cn

TS:   console.assert(x > 0);
来源：http://qhk.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://dtg.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vkj.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cff.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://twz.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://hcb.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://xpy.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rkk.pycfn.com

JS:   e.message;  e.stack
来源：http://qyt.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfs.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://flh.fanxiaobao.xyz

Go:   err.Error()
来源：http://iow.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://doj.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://fhw.snrcjt.cn

[H09] 带错误码的异常
来源：http://peq.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tef.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tmc.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ics.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://exe.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jpx.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wzj.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pdu.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uen.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://klr.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zje.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wql.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vsi.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wfv.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oem.jlsjyb.cn

Go:   defer f.Close()
来源：http://lzc.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzk.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aae.meibo888.top

================================================================================
来源：http://jcm.yfazqb.com

I. 正则表达式
来源：http://lqo.ivvv.top

================================================================================
来源：http://yrs.cheryme.top

[I01] 判断是否匹配
来源：http://ftv.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdz.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://hik.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://rrn.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://ltl.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mgz.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ilk.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://hsm.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vyc.bbcook.cn

[I02] 提取所有匹配
来源：http://riv.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://mlo.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fqb.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://flj.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://gve.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyw.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://akk.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://ppe.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dct.c1oappe.top

[I03] 提取捕获分组
来源：http://aki.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rfg.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kat.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dpz.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://atx.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ugz.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://abq.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cfy.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ntl.hfpthk.cn

[I04] 正则替换
来源：http://jtz.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kjk.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rhy.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://rdp.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mvw.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ajb.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://phg.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zox.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ipw.yj202588.top

[I05] 按正则拆分
来源：http://hvu.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cne.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rul.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://xxb.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://wll.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://tzc.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ihw.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zuh.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qfb.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pax.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tor.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wcu.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfu.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oed.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://azf.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ncr.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gki.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://net.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://lsm.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wdm.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bcr.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nwr.ydzc1.top

TS:   /error/gim
来源：http://nol.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kpr.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dms.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://cmc.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hiw.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://yhu.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrg.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ajj.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://azs.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://giy.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mww.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vpt.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qil.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nhd.nanxuanxn.top

================================================================================
来源：http://kth.yfazqb.com

J. 日期与时间
来源：http://rav.vqdsnc.cn

================================================================================
来源：http://qeb.nanxinkj.top

[J01] 获取当前时间
来源：http://xao.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://auv.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tur.nwbrower.top

JS:   new Date();  Date.now()
来源：http://qcm.fengsongda.top

TS:   new Date();  Date.now()
来源：http://ufu.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uwn.zdqjudy.top

Go:   time.Now()
来源：http://wsa.guowangkeji.top

Ruby: Time.now
来源：http://hen.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sub.shzxlz.cn

[J02] 格式化输出
来源：http://azu.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://naz.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://klk.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lhv.hongshengwenyu.top

TS:   d.toISOString()
来源：http://qrl.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ikx.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bke.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnc.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zzy.xylfe.cn

[J03] 字符串解析为日期
来源：http://kty.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pfx.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sje.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://dwh.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://mpj.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://qpn.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mml.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://mxo.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gxk.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://gpr.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nzt.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://deu.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sbi.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://nhk.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oct.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rlz.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://civ.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mmf.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://nii.yj20258.top

Py:   now + timedelta(days=7)
来源：http://hhq.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ztw.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbx.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vtg.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://fmb.daria6918.cn


<!-- 参考信息 -->