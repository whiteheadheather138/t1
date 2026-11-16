代发 wailian999

JS:   this.name = "x";
来源：http://pjm.gotoacloud.top

TS:   name: string = "x";
来源：http://hyl.xylfe.cn

Java: private String name;
来源：http://clu.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bsg.dashuyun.cn

Ruby: @name = "x"
来源：http://ofz.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://pmj.guowangkeji.top

[G04] 定义方法
来源：http://iuv.pycfn.com

Py:   def greet(self): return self.name
来源：http://szn.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://tjx.yj20258.top

JS:   greet() { return this.name; }
来源：http://ypg.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://eol.havefunace.top

Java: String greet() { return name; }
来源：http://jwm.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ilx.gogol.net.cn

Ruby: def greet; @name; end
来源：http://ujx.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://rvk.shangyingyoupin.top

[G05] 继承
来源：http://tga.cheryme.top

Py:   class Admin(User): pass
来源：http://vwe.hcnkem.com

PHP:  class Admin extends User {}
来源：http://bwf.yonumen.top

JS:   class Admin extends User {}
来源：http://xeh.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://ick.vqdsnc.cn

Java: class Admin extends User {}
来源：http://xha.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mmr.uphjek.com

Ruby: class Admin < User; end
来源：http://elt.xziqi.cn

C#:   class Admin : User {}
来源：http://rag.jinyuanbaomall.cn

[G06] 重写方法
来源：http://ehf.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://svr.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qcz.yj20258.top

JS:   greet() { return "admin"; }
来源：http://naj.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://awz.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://wcp.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rdr.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://yxf.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://kwx.yfazqb.com

[G07] 调用父类方法
来源：http://pid.guannengcc.top

Py:   super().greet()
来源：http://wqh.hfpthk.cn

PHP:  parent::greet();
来源：http://hpj.zhaomingkeji.xyz

JS:   super.greet();
来源：http://cuw.zhiwuduotai.top

TS:   super.greet();
来源：http://bep.havefunace.top

Java: super.greet();
来源：http://sqn.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vkv.uphjek.com

Ruby: super
来源：http://fyi.ybcxt.top

C#:   base.Greet();
来源：http://fai.fengsongda.top

[G08] 静态方法与属性
来源：http://jgp.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tiy.jqgufenzy.top

PHP:  public static function f() {}
来源：http://zic.chenzaomai.com

JS:   static f() {}
来源：http://lng.c1oappe.top

TS:   static f(): void {}
来源：http://ogf.redwolf501.top

Java: static void f() {}
来源：http://prd.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kmj.aizwys.cn

Ruby: def self.f; end
来源：http://zvg.yvedp.cn

C#:   public static void F() {}
来源：http://stm.daxiang520.top

[G09] 接口 / 抽象类
来源：http://doi.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://uwa.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qkd.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ozn.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://sks.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://uwm.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ieo.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ofp.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://zvg.ctjpmb.com

[G10] 访问控制
来源：http://zgt.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://itc.yj20258.top

PHP:  public / protected / private
来源：http://dwh.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://qba.guowangkeji.top

TS:   public / protected / private
来源：http://qxt.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://azn.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qqd.zhengqikj.top

Ruby: public / protected / private
来源：http://ksk.jiagoushi.top

C#:   public / protected / private / internal
来源：http://tou.sysykeji.top

[G11] getter / setter
来源：http://vow.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://ssk.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qil.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://xvb.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://oze.tanke756.top

Java: public String getName() { return name; }
来源：http://nzo.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lmy.sufxvd.cn

Ruby: attr_accessor :name
来源：http://wel.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://qak.jinqigufen.top

[G12] 对象转字符串
来源：http://bbe.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://qst.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bwb.yongpay.top

JS:   toString() { return this.name; }
来源：http://pnc.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://hdd.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://dqf.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://juu.yfazqb.com

Ruby: def to_s; @name; end
来源：http://oth.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://ebf.ydzc1.top

[G13] 判断对象类型
来源：http://luh.chenlongwang.top

Py:   isinstance(u, User)
来源：http://mry.cqqwz.cn

PHP:  $u instanceof User
来源：http://kap.yvedp.cn

JS:   u instanceof User
来源：http://qbx.jianghu66.top

TS:   u instanceof User
来源：http://mgd.ppjwa.cn

Java: u instanceof User
来源：http://nqx.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zpz.aizwys.cn

Ruby: u.is_a?(User)
来源：http://ukk.daxiang520.top

C#:   u is User
来源：http://xvi.ydjk.org.cn

[G14] 数据类 / record
来源：http://yyz.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gir.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://knj.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xcb.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://mbb.wangdashe.top

Java: record User(String name, int age) {}
来源：http://ein.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://kcr.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://czn.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://chh.shanyushiyangtech.top

[G15] 枚举
来源：http://zci.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hfy.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yiy.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wws.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://byx.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://kzl.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fky.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://sha.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ogs.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://xpv.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yxv.yj20258.top

PHP:  get_object_vars($obj);
来源：http://mtq.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://azv.dashuyun.cn

TS:   Object.entries(obj)
来源：http://qas.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ryt.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vjd.daria6918.cn

Ruby: obj.instance_variables
来源：http://jsm.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://vfa.ydjk.org.cn

================================================================================
来源：http://uog.nwbrower.top

H. 异常与错误处理
来源：http://rfp.cashguo.top

================================================================================
来源：http://eda.zhengqikj.top

[H01] try / catch 基础
来源：http://ogk.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blr.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://clm.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nye.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxh.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qjf.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://afk.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hge.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ode.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://lmu.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://nfs.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sga.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://heu.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lul.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vrf.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ont.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://vxn.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fcr.sweek.top

[H03] 主动抛出异常
来源：http://jtq.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://jvs.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ptv.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://gfk.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://qwg.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ool.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vrk.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vos.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://dof.tian-w.cn

[H04] 自定义异常类型
来源：http://tfb.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://rin.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://uec.yj20258888.top

JS:   class MyError extends Error {}
来源：http://jiq.cashguo.top

TS:   class MyError extends Error {}
来源：http://wgp.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ziw.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ldr.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://bmr.hcnkem.com

C#:   class MyException : Exception {}
来源：http://qne.bjfxy.top

[H05] 捕获特定类型
来源：http://hkm.jianghu66.top

Py:   except ValueError as e:
来源：http://hna.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfe.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vyw.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://ner.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://pvu.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vkp.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://hvg.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lbt.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://vmi.xylfe.cn

Py:   value = d.get("k") or default
来源：http://rai.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://gxi.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://uya.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://qvu.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hww.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qzx.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://xew.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://qgs.tanke756.top

[H07] 断言
来源：http://cke.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://jvr.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://aqd.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://bhw.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://dbg.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://vtq.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wrs.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://wkj.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://wvk.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://anb.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://qlx.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vht.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://yyr.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tut.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rzy.yuxming.cn

Go:   err.Error()
来源：http://pjg.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://oex.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://oyc.zhongyouzk.top

[H09] 带错误码的异常
来源：http://vsm.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nhc.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vua.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://efj.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xnx.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yhx.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fmt.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://boj.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://njs.dashuyun.cn

[H10] 资源自动释放
来源：http://osh.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pew.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rqv.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zbb.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nfy.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bwc.zhongyouzk.top

Go:   defer f.Close()
来源：http://qst.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ywd.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hzo.hnqzz.top

================================================================================
来源：http://vin.zycfv.cn

I. 正则表达式
来源：http://ttw.fengsongda.top

================================================================================
来源：http://hme.jlsjyb.cn

[I01] 判断是否匹配
来源：http://abf.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewp.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nxt.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://yqe.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://wka.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://liy.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fto.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://qxz.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rhg.kuanghao11.cn

[I02] 提取所有匹配
来源：http://bfg.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://bgt.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gbf.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xeb.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://ury.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ana.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wgn.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://rse.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgl.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://bgr.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rbq.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://two.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jty.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fox.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://att.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wws.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://epf.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vvd.hysaishi.cn

[I04] 正则替换
来源：http://jdf.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://rhy.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://prz.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://xfk.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uvf.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://szb.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://opn.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://qhm.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qef.sysykeji.top

[I05] 按正则拆分
来源：http://hxa.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pce.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wah.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://pul.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://osj.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://kfg.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zhn.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://zac.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vcp.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pdv.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vys.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://obk.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mnl.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uau.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhw.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehr.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ccm.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://saq.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://jxs.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lwr.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cix.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yzc.sweek.top

TS:   /error/gim
来源：http://gid.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://trl.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aru.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://ghi.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://djg.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://lnj.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wyk.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oue.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jkv.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmi.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vad.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rtc.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xpg.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jum.bjfxy.top

================================================================================
来源：http://rot.epnwcf.com

J. 日期与时间
来源：http://nef.xingfuxueyuan.xyz

================================================================================
来源：http://bov.hywenlv.cn

[J01] 获取当前时间
来源：http://obo.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wbd.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gpx.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://jcw.xziqi.cn

TS:   new Date();  Date.now()
来源：http://djw.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ldm.wangdashe.top


<!-- 参考信息 -->