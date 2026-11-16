代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hjr.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://hci.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://jye.uphjek.com

Java: String greet() { return name; }
来源：http://bgh.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gha.hcnkem.com

Ruby: def greet; @name; end
来源：http://gvo.yj20258888.top

C#:   public string Greet() => Name;
来源：http://zbp.hywenlv.cn

[G05] 继承
来源：http://lcg.gogol.net.cn

Py:   class Admin(User): pass
来源：http://dan.tanke756.top

PHP:  class Admin extends User {}
来源：http://pwy.hywenlv.cn

JS:   class Admin extends User {}
来源：http://kli.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://dic.bjfxy.top

Java: class Admin extends User {}
来源：http://nbl.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://emz.zdbjq.cn

Ruby: class Admin < User; end
来源：http://gei.jqgfzy.top

C#:   class Admin : User {}
来源：http://ava.jqgfzy.top

[G06] 重写方法
来源：http://ipo.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://eef.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ecn.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://gfw.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://lcc.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://cqh.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://okc.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://jdx.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://vxy.epnwcf.com

[G07] 调用父类方法
来源：http://haa.aizwys.cn

Py:   super().greet()
来源：http://cvf.svipenyu.cn

PHP:  parent::greet();
来源：http://zzh.yvedp.cn

JS:   super.greet();
来源：http://maf.epnwcf.com

TS:   super.greet();
来源：http://gkx.9152youxi.cn

Java: super.greet();
来源：http://ahm.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://txa.jianghu66.top

Ruby: super
来源：http://cxy.wangshuangyany.cn

C#:   base.Greet();
来源：http://lin.9152youxi.cn

[G08] 静态方法与属性
来源：http://ffi.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ljv.cheryme.top

PHP:  public static function f() {}
来源：http://oqh.yj202588.top

JS:   static f() {}
来源：http://qqc.guannengcc.top

TS:   static f(): void {}
来源：http://sgd.shuidangran.top

Java: static void f() {}
来源：http://ome.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://kte.hysaishi.cn

Ruby: def self.f; end
来源：http://lqa.snrcjt.cn

C#:   public static void F() {}
来源：http://jpy.xuanzx.com

[G09] 接口 / 抽象类
来源：http://fwt.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pdy.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://klk.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://dip.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://ene.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://vji.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://krd.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jmq.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://hbd.tianlin.xyz

[G10] 访问控制
来源：http://lrr.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://xvb.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://fga.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://eov.tarul.cn

TS:   public / protected / private
来源：http://mwx.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://iex.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fmc.xziqi.cn

Ruby: public / protected / private
来源：http://ktx.xuanzx.com

C#:   public / protected / private / internal
来源：http://nee.ctjpmb.com

[G11] getter / setter
来源：http://qep.xziqi.cn

Py:   @property 与 @x.setter
来源：http://cvq.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cfe.daria6918.cn

JS:   get name() { return this._name; }
来源：http://vrd.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://pso.hywenlv.cn

Java: public String getName() { return name; }
来源：http://ljf.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbm.tianlin.xyz

Ruby: attr_accessor :name
来源：http://wlx.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://bbp.yangfankeji.com

[G12] 对象转字符串
来源：http://omn.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://cug.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tik.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://fyy.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://sjt.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://aff.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://wow.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://nrs.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://meq.gogol.net.cn

[G13] 判断对象类型
来源：http://www.nwbrower.top

Py:   isinstance(u, User)
来源：http://nuc.bjfxy.top

PHP:  $u instanceof User
来源：http://sps.hnqzz.top

JS:   u instanceof User
来源：http://mqr.yueranfly.top

TS:   u instanceof User
来源：http://zlw.yfazqb.com

Java: u instanceof User
来源：http://oce.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kdn.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://xsf.tarul.cn

C#:   u is User
来源：http://fnp.zdqjudy.top

[G14] 数据类 / record
来源：http://hny.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://haf.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://llc.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://aqk.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://mfy.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://zgv.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://ezo.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcf.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://xcn.epnwcf.com

[G15] 枚举
来源：http://lvn.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://afq.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kxr.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jvr.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jxr.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://sjs.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rty.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://puj.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ggf.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://nik.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cef.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://iht.dashuyun.cn

JS:   Object.entries(obj)
来源：http://ytl.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://wvs.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://irb.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://twl.yuxming.cn

Ruby: obj.instance_variables
来源：http://uva.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://apu.yuxming.cn

================================================================================
来源：http://vpz.nanxinkj.top

H. 异常与错误处理
来源：http://gkk.ctjpmb.com

================================================================================
来源：http://ghe.chenlongwang.top

[H01] try / catch 基础
来源：http://wnp.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vte.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mzg.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hci.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://duu.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajr.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lxa.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dec.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://geo.redwolf501.top

[H02] finally / ensure 收尾
来源：http://klg.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://ozq.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ogq.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://toj.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://fsr.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://doj.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ith.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eye.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://srb.yanxiufei.cn

[H03] 主动抛出异常
来源：http://sck.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://hfm.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tfh.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://gru.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://whx.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yro.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mtd.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rvi.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://enj.9152youxi.cn

[H04] 自定义异常类型
来源：http://mal.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://gzy.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://zap.ybcxt.top

JS:   class MyError extends Error {}
来源：http://dgp.epnwcf.com

TS:   class MyError extends Error {}
来源：http://iyu.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://uuk.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ttc.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://ldg.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://bmp.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://csb.hnqzz.top

Py:   except ValueError as e:
来源：http://adh.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nml.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://vqg.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://amb.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://keq.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://phb.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://gbz.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ttj.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://tht.gzhubu.top

Py:   value = d.get("k") or default
来源：http://xcw.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nbw.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://syu.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://ypg.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://opz.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://onu.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://jit.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://dlk.svipenyu.cn

[H07] 断言
来源：http://ovo.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://wzq.snrcjt.cn

PHP:  assert($x > 0);
来源：http://axh.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://qks.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://tgw.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://eny.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lwk.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xju.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://jsz.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://mek.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://fvh.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wyx.jqgfzy.top

JS:   e.message;  e.stack
来源：http://wbx.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pnq.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eru.sysykeji.top

Go:   err.Error()
来源：http://wal.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://hsc.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://ktf.yueranfly.top

[H09] 带错误码的异常
来源：http://odu.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mmw.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hyx.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rgs.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uax.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qic.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aoj.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://odt.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kio.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://ikk.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://fuk.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ktp.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kwd.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ftd.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://glh.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://htf.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://abj.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qst.yvedp.cn

================================================================================
来源：http://wkr.fktsv.cn

I. 正则表达式
来源：http://jxw.zhijiandao.cn

================================================================================
来源：http://oup.jinqigfzy.top

[I01] 判断是否匹配
来源：http://zgs.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baq.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://svb.havefunace.top

JS:   /\d+/.test(s)
来源：http://vhz.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://yig.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uqn.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyt.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://ket.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://drp.havefunace.top

[I02] 提取所有匹配
来源：http://rdd.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://mlk.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ski.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pyq.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://ujv.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aar.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://soo.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://ljn.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lxq.zhixingplan.top

[I03] 提取捕获分组
来源：http://nfj.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uvs.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rft.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://htw.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xjn.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hxq.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jqs.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oks.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jql.nanxuanxn.top

[I04] 正则替换
来源：http://rol.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://phk.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xcp.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fgj.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://zui.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://ded.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://did.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vrt.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tsm.zhiwuduotai.top

[I05] 按正则拆分
来源：http://pjy.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dfy.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yqz.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://avb.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://fsm.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://qao.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rse.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://mdb.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgs.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hrk.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aju.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ojm.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsp.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwa.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bvb.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uil.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://agn.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lks.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://maz.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://akp.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kzz.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vft.yj20258888.top

TS:   /error/gim
来源：http://xzh.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://izn.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zbg.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://iha.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vjn.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ctx.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aqg.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oaz.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnj.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kap.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sno.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://loc.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://krn.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wdg.sweek.top

================================================================================
来源：http://vff.tanke756.top

J. 日期与时间
来源：http://cbd.gotoacloud.top

================================================================================
来源：http://gsz.ppjwa.cn

[J01] 获取当前时间
来源：http://ava.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ohl.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blh.aizwys.cn

JS:   new Date();  Date.now()
来源：http://yfp.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://eqk.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jvk.xuanzx.com

Go:   time.Now()
来源：http://daz.epnwcf.com

Ruby: Time.now
来源：http://nlk.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmt.ybcxt.top

[J02] 格式化输出
来源：http://uqi.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxl.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xiz.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vgq.zhoulong.xyz

TS:   d.toISOString()
来源：http://aww.nanxinkj.top


<!-- 参考信息 -->