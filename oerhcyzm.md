代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://owh.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://tio.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://jul.fehbvm.com

[G05] 继承
来源：http://twn.yuxming.cn

Py:   class Admin(User): pass
来源：http://bnr.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://vjo.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://dkh.jyoumei.cn

TS:   class Admin extends User {}
来源：http://rei.ehwqpu.com

Java: class Admin extends User {}
来源：http://yzd.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tei.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://wwb.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://dgs.feifeiyinyue.top

[G06] 重写方法
来源：http://lqv.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://ccf.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://unc.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://vsd.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://axm.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://bjj.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://enl.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://rlj.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://ide.zhixingplan.top

[G07] 调用父类方法
来源：http://avt.fktsv.cn

Py:   super().greet()
来源：http://aqe.fktsv.cn

PHP:  parent::greet();
来源：http://zcj.fengsongda.top

JS:   super.greet();
来源：http://pfg.ydzc1.top

TS:   super.greet();
来源：http://fhp.ehwqpu.com

Java: super.greet();
来源：http://bpc.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hpp.shangyingyoupin.top

Ruby: super
来源：http://lxh.redwolf501.top

C#:   base.Greet();
来源：http://lrj.fengsongda.top

[G08] 静态方法与属性
来源：http://rmb.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xst.yuanzhike.top

PHP:  public static function f() {}
来源：http://vwh.fehbvm.com

JS:   static f() {}
来源：http://pms.yanxiufei.cn

TS:   static f(): void {}
来源：http://nca.mhx1999.top

Java: static void f() {}
来源：http://xtf.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ueg.aibaodan.cn

Ruby: def self.f; end
来源：http://rva.chenlongwang.top

C#:   public static void F() {}
来源：http://lti.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://tkx.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://omc.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://uky.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hve.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://bzj.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://sns.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://erb.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ozp.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://vna.jinyuanbaomall.cn

[G10] 访问控制
来源：http://bbi.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ycb.yanxiufei.cn

PHP:  public / protected / private
来源：http://wrr.sweek.top

JS:   #private 字段；其余公开
来源：http://vyo.xinyue.icu

TS:   public / protected / private
来源：http://cyv.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://cyo.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryd.shzxlz.cn

Ruby: public / protected / private
来源：http://oii.tian-w.cn

C#:   public / protected / private / internal
来源：http://vri.vqdsnc.cn

[G11] getter / setter
来源：http://oub.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://jbp.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qri.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://xxv.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://pbo.9152youxi.cn

Java: public String getName() { return name; }
来源：http://ytt.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://ovl.haohaochexian.top

Ruby: attr_accessor :name
来源：http://xjm.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://dpp.cashguo.top

[G12] 对象转字符串
来源：http://zmb.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://opt.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rvy.gzhubu.top

JS:   toString() { return this.name; }
来源：http://edp.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://krn.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://uwu.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://ant.yfazqb.com

Ruby: def to_s; @name; end
来源：http://wmt.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://qni.jinqigufen.top

[G13] 判断对象类型
来源：http://iwv.dianchejie.cn

Py:   isinstance(u, User)
来源：http://rwg.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://snv.cucudq.cn

JS:   u instanceof User
来源：http://mfj.shuidangran.top

TS:   u instanceof User
来源：http://owq.xuanzx.com

Java: u instanceof User
来源：http://bcq.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://mwb.sweek.top

Ruby: u.is_a?(User)
来源：http://uwh.jqgufenzy.top

C#:   u is User
来源：http://dhk.fktsv.cn

[G14] 数据类 / record
来源：http://tld.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qns.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://txf.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://izu.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://vui.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://usf.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://zgx.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rjn.yj202588.top

C#:   record User(string Name, int Age);
来源：http://dsf.zdqjudy.top

[G15] 枚举
来源：http://kht.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pjw.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://idk.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zdf.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rbb.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://nxa.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zda.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://kdx.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sfw.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://gcs.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qwx.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://szo.xylfe.cn

JS:   Object.entries(obj)
来源：http://msd.cheryme.top

TS:   Object.entries(obj)
来源：http://igp.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yiw.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqg.zhengqikj.top

Ruby: obj.instance_variables
来源：http://fli.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://yor.sjlbkw.cn

================================================================================
来源：http://ygw.sysykeji.top

H. 异常与错误处理
来源：http://npf.gaohongyu789.top

================================================================================
来源：http://kvj.zhoulong.xyz

[H01] try / catch 基础
来源：http://vwd.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rbm.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ogv.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puk.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mdt.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vlf.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lei.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jom.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkk.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://vze.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://toj.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mij.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ock.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vde.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://trq.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://obl.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://zjq.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oqk.yueranfly.top

[H03] 主动抛出异常
来源：http://suw.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://qmr.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mgx.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://qxp.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://ppd.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jze.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eyj.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pcm.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ntt.yangfankeji.com

[H04] 自定义异常类型
来源：http://tei.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://abu.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://xby.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://ifu.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://fhf.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://tzw.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pci.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://qpx.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://kdp.ctjpmb.com

[H05] 捕获特定类型
来源：http://oeb.fehbvm.com

Py:   except ValueError as e:
来源：http://rpw.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pfn.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://hmz.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://fdr.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://wvz.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nno.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://bts.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwb.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://nlb.nwbrower.top

Py:   value = d.get("k") or default
来源：http://fen.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jcg.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://uaz.pycfn.com

TS:   obj?.a?.b;  d ?? default
来源：http://lhx.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://opy.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qfd.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://iqm.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://pki.andypj.xyz

[H07] 断言
来源：http://guz.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://zls.jinqigufen.top

PHP:  assert($x > 0);
来源：http://nyz.wangdashe.top

JS:   console.assert(x > 0);
来源：http://vbg.xuanzx.com

TS:   console.assert(x > 0);
来源：http://leg.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://gxo.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gce.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://eku.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://kso.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://dgm.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://utz.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cri.vehdjk.com

JS:   e.message;  e.stack
来源：http://dig.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://fbi.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tdv.mhx1999.top

Go:   err.Error()
来源：http://rhc.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://eiz.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://uxl.sxryk.cn

[H09] 带错误码的异常
来源：http://vis.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://icx.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://aol.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jku.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://guf.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://caq.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xvb.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://hdm.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uwh.sxryk.cn

[H10] 资源自动释放
来源：http://wev.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iro.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zsk.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cen.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcv.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fjh.zhijiandao.cn

Go:   defer f.Close()
来源：http://ahh.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hqk.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lwc.jianghu66.top

================================================================================
来源：http://lkg.jqgfzy.top

I. 正则表达式
来源：http://roh.yanxiufei.cn

================================================================================
来源：http://mlg.ctjpmb.com

[I01] 判断是否匹配
来源：http://nrh.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fri.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://obv.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://hvm.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://bpg.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pim.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dtp.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://dih.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zwa.xinyue.icu

[I02] 提取所有匹配
来源：http://vpa.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://yqh.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://frh.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lre.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://uka.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyq.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sjd.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://rfl.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kse.hcnkem.com

[I03] 提取捕获分组
来源：http://ehm.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xqf.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xvd.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wtj.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vts.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lhj.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nci.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://toj.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wvu.yueranfly.top

[I04] 正则替换
来源：http://ltn.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mxe.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufa.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://kkz.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://niw.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://hap.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://epz.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gep.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xng.fzhhl.top

[I05] 按正则拆分
来源：http://qad.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fkk.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yrm.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://pst.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://kwr.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://qzx.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hre.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://drq.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qcg.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kpj.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pye.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lkt.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdj.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osb.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fch.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ozm.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://edi.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qhj.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://tba.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lgo.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://crc.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rzc.sysykeji.top

TS:   /error/gim
来源：http://emt.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dke.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jyw.zhiwuduotai.top

Ruby: s.scan(/error/i)
来源：http://pgr.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hyp.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://pzf.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ufu.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lys.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkq.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xgn.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://yfr.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xtl.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ooz.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lqa.xuanzx.com

================================================================================
来源：http://gud.yfazqb.com

J. 日期与时间
来源：http://bxe.sjlbkw.cn

================================================================================
来源：http://xng.pycfn.com

[J01] 获取当前时间
来源：http://xcf.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tbj.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mkk.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://tvm.bbcook.cn

TS:   new Date();  Date.now()
来源：http://jui.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zre.haohaochexian.top

Go:   time.Now()
来源：http://urs.jinyuanbaomall.cn

Ruby: Time.now
来源：http://gfc.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fov.ydzc1.top

[J02] 格式化输出
来源：http://xhi.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfn.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pir.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cmo.dianchejie.cn

TS:   d.toISOString()
来源：http://fms.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ndj.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lmo.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwk.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mdm.jinghuilouyu.cn


<!-- 参考信息 -->