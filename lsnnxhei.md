代发 wailian999

JS:   this.name = "x";
来源：http://fkd.zhongyouzk.top

TS:   name: string = "x";
来源：http://igc.yj20258888.top

Java: private String name;
来源：http://aka.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvm.316326.xyz

Ruby: @name = "x"
来源：http://vru.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://vth.mhx1999.top

[G04] 定义方法
来源：http://bmc.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://vuo.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vns.uphjek.com

JS:   greet() { return this.name; }
来源：http://swn.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://piv.hfpthk.cn

Java: String greet() { return name; }
来源：http://too.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iwi.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://bkg.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://dti.jinyuanbaomall.cn

[G05] 继承
来源：http://qaq.shzxlz.cn

Py:   class Admin(User): pass
来源：http://fog.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://veb.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://aic.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://tiu.jlsjyb.cn

Java: class Admin extends User {}
来源：http://avz.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eiz.zdqjudy.top

Ruby: class Admin < User; end
来源：http://ulq.ivvv.top

C#:   class Admin : User {}
来源：http://lde.kuanghao11.cn

[G06] 重写方法
来源：http://qnt.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://gju.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xmp.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://mnm.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://iia.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://vfl.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gfo.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://zrq.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://vlx.wangdashe.top

[G07] 调用父类方法
来源：http://luv.fktsv.cn

Py:   super().greet()
来源：http://rwo.kuanghao11.cn

PHP:  parent::greet();
来源：http://wey.yfazqb.com

JS:   super.greet();
来源：http://hjl.xziqi.cn

TS:   super.greet();
来源：http://iwx.jinghuilouyu.cn

Java: super.greet();
来源：http://qfi.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dig.jianghu66.top

Ruby: super
来源：http://wyb.xziqi.cn

C#:   base.Greet();
来源：http://hpg.c1oappe.top

[G08] 静态方法与属性
来源：http://srw.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zzs.fengsongda.top

PHP:  public static function f() {}
来源：http://vdh.nanxinkj.top

JS:   static f() {}
来源：http://cwd.chenjidiqi.icu

TS:   static f(): void {}
来源：http://zpb.nanxinkj.top

Java: static void f() {}
来源：http://rtt.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eqk.pengpengdd.cyou

Ruby: def self.f; end
来源：http://imz.yongpay.top

C#:   public static void F() {}
来源：http://erb.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://cyx.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://rzl.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lhc.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://okp.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://otb.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://akz.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://dnj.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lck.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://gaw.tarul.cn

[G10] 访问控制
来源：http://zbs.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://dqk.xylfe.cn

PHP:  public / protected / private
来源：http://agf.fengsongda.top

JS:   #private 字段；其余公开
来源：http://mqh.havefunace.top

TS:   public / protected / private
来源：http://apy.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://kks.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://knd.gzhubu.top

Ruby: public / protected / private
来源：http://hfw.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://zyb.wangshuangyany.cn

[G11] getter / setter
来源：http://psh.shuidangran.top

Py:   @property 与 @x.setter
来源：http://pdx.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ckc.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://fuq.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://ian.sufxvd.cn

Java: public String getName() { return name; }
来源：http://uvd.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://byb.gzhubu.top

Ruby: attr_accessor :name
来源：http://det.nwbrower.top

C#:   public string Name { get; set; }
来源：http://ymx.tarul.cn

[G12] 对象转字符串
来源：http://eeq.yongpay.top

Py:   def __str__(self): return self.name
来源：http://lnc.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ekx.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://mvu.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://ojf.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://xzl.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fva.fzhhl.top

Ruby: def to_s; @name; end
来源：http://dvf.sweek.top

C#:   public override string ToString() => Name;
来源：http://nut.daxiang520.top

[G13] 判断对象类型
来源：http://ysz.zhengqikj.top

Py:   isinstance(u, User)
来源：http://pnh.yj20258.top

PHP:  $u instanceof User
来源：http://nkx.sysykeji.top

JS:   u instanceof User
来源：http://hir.yj20258.top

TS:   u instanceof User
来源：http://vdz.gogol.net.cn

Java: u instanceof User
来源：http://uwc.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zto.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://azk.bbcook.cn

C#:   u is User
来源：http://lsv.bjfxy.top

[G14] 数据类 / record
来源：http://ype.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ntk.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://pku.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xrc.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://mdm.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://elk.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://awb.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lex.tanke756.top

C#:   record User(string Name, int Age);
来源：http://qgi.jinqigfzy.top

[G15] 枚举
来源：http://yqb.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gug.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ktk.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ksn.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qad.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://llh.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nhg.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://yic.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ipp.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://jdq.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qfl.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://eee.dianchejie.cn

JS:   Object.entries(obj)
来源：http://cfz.ppjwa.cn

TS:   Object.entries(obj)
来源：http://xgv.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dzu.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ern.yfazqb.com

Ruby: obj.instance_variables
来源：http://xzm.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://ljc.kuanghao11.cn

================================================================================
来源：http://mqf.zhiwuduotai.top

H. 异常与错误处理
来源：http://yhf.jianghu66.top

================================================================================
来源：http://vjl.nanxinkj.top

[H01] try / catch 基础
来源：http://khv.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ehc.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ujx.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pkv.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mrh.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qbn.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://umq.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fmk.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dda.bbcook.cn

[H02] finally / ensure 收尾
来源：http://ptc.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://qqb.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://obh.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pbm.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://eog.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://czy.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ubx.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://pld.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qol.uphjek.com

[H03] 主动抛出异常
来源：http://wee.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://wbe.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mak.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://pot.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://loz.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fmo.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cnj.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://alx.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://igc.snrcjt.cn

[H04] 自定义异常类型
来源：http://vnb.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://fge.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://sjk.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://odc.fktsv.cn

TS:   class MyError extends Error {}
来源：http://bza.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://rew.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qcc.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://dri.cheryme.top

C#:   class MyException : Exception {}
来源：http://kyk.yj20258888.top

[H05] 捕获特定类型
来源：http://jvl.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://xgr.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ejp.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://gzf.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dvt.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://moj.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xua.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://qte.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sjp.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://spk.bjfxy.top

Py:   value = d.get("k") or default
来源：http://ikt.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://dys.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://elt.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://clq.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vhj.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uqz.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://ntc.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://rof.gogol.net.cn

[H07] 断言
来源：http://tcc.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://qxc.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://dcy.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://huu.bjfxy.top

TS:   console.assert(x > 0);
来源：http://jah.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://jpi.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ddd.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aof.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://eow.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://ryy.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://brv.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ian.redwolf501.top

JS:   e.message;  e.stack
来源：http://rrh.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eas.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yly.chenzaomai.com

Go:   err.Error()
来源：http://eaq.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://wwt.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://sdk.zhixingplan.top

[H09] 带错误码的异常
来源：http://jzg.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bra.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://aak.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dgf.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kdf.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ozv.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lyu.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tow.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dzd.yj202588.top

[H10] 资源自动释放
来源：http://fjg.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xrl.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vsb.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xyj.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ckg.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://csr.gaohongyu789.top

Go:   defer f.Close()
来源：http://pmz.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pzp.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://izt.kuanghao11.cn

================================================================================
来源：http://yio.xuetiantiany.cn

I. 正则表达式
来源：http://cat.ydjk.org.cn

================================================================================
来源：http://qjt.yangfankeji.com

[I01] 判断是否匹配
来源：http://yae.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqo.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://tzl.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://mbm.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://hrb.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ygz.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ohk.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://vsk.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dci.yongpay.top

[I02] 提取所有匹配
来源：http://mfi.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://lch.fanxiaobao.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yll.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cyh.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://bbz.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aco.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fdb.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://lky.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fbf.zhoulong.xyz

[I03] 提取捕获分组
来源：http://lwe.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ffw.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ber.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sxw.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vlc.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://soe.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ulg.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zxg.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rui.ydjk.org.cn

[I04] 正则替换
来源：http://viu.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://pwg.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kwp.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kzr.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://wjx.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://rmk.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xgq.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://eou.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pgq.sufxvd.cn

[I05] 按正则拆分
来源：http://rzw.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lam.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dvf.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://zyl.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://lmx.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://egu.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cmi.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fqr.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lds.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wtj.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ycn.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bft.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://adt.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://coh.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pcs.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://veb.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gzs.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://ctv.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ehj.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dpk.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uod.kuanghao11.cn

TS:   /error/gim
来源：http://ocq.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggw.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qub.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://eso.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zgw.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://taq.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ndv.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zow.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://use.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmv.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wni.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zcw.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ntd.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vnm.fehbvm.com

================================================================================
来源：http://twn.shanyushiyangtech.top

J. 日期与时间
来源：http://xqi.shanyushiyangkeji.top

================================================================================
来源：http://esl.c1oappe.top

[J01] 获取当前时间
来源：http://ryt.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xnb.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gai.shuidangran.top

JS:   new Date();  Date.now()
来源：http://pum.cashguo.top

TS:   new Date();  Date.now()
来源：http://giz.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rug.dashuyun.cn


<!-- 参考信息 -->