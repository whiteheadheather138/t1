代发 wailian999

Ruby: @name = "x"
来源：http://ude.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://dfp.ydzc1.top

[G04] 定义方法
来源：http://ykg.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://zcq.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hes.52xcode.cn

JS:   greet() { return this.name; }
来源：http://ksh.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://qgs.daria6918.cn

Java: String greet() { return name; }
来源：http://swc.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fnf.sysykeji.top

Ruby: def greet; @name; end
来源：http://vwo.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://dmk.yj20258888.top

[G05] 继承
来源：http://gzf.aibaodan.cn

Py:   class Admin(User): pass
来源：http://ffl.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://jtj.aibaodan.cn

JS:   class Admin extends User {}
来源：http://etc.zhixingplan.top

TS:   class Admin extends User {}
来源：http://bfx.guannengcc.top

Java: class Admin extends User {}
来源：http://npc.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pgu.hesvh.cn

Ruby: class Admin < User; end
来源：http://fir.zycfv.cn

C#:   class Admin : User {}
来源：http://urm.cashguo.top

[G06] 重写方法
来源：http://gkw.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://sia.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dxx.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://uuy.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://gpg.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://tug.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yow.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://plg.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://zul.zhoulong.xyz

[G07] 调用父类方法
来源：http://czv.yongpay.top

Py:   super().greet()
来源：http://vym.wangshuangyany.cn

PHP:  parent::greet();
来源：http://arx.yj20258.top

JS:   super.greet();
来源：http://cil.haohaochexian.top

TS:   super.greet();
来源：http://bqg.bjfxy.top

Java: super.greet();
来源：http://wxx.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gpo.chenlongwang.top

Ruby: super
来源：http://uoc.sxryk.cn

C#:   base.Greet();
来源：http://nlm.cucudq.cn

[G08] 静态方法与属性
来源：http://kdt.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aaf.tian-w.cn

PHP:  public static function f() {}
来源：http://aow.cdnleiting.top

JS:   static f() {}
来源：http://oqv.gaohongyu789.top

TS:   static f(): void {}
来源：http://cde.316326.xyz

Java: static void f() {}
来源：http://ddd.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wel.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://ieg.aibaodan.cn

C#:   public static void F() {}
来源：http://fcy.andypj.xyz

[G09] 接口 / 抽象类
来源：http://nhg.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://hsl.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://upi.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ccc.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://bag.hammf.cn

Java: interface Shape { double area(); }
来源：http://lqj.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://zon.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://myd.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://ohw.nwbrower.top

[G10] 访问控制
来源：http://xjr.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://usy.chenjidiqi.icu

PHP:  public / protected / private
来源：http://gfm.xuanzx.com

JS:   #private 字段；其余公开
来源：http://mro.jinqigufen.top

TS:   public / protected / private
来源：http://xbl.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://gbf.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qjw.quarkkingdee.top

Ruby: public / protected / private
来源：http://dss.cashguo.top

C#:   public / protected / private / internal
来源：http://llm.gogol.net.cn

[G11] getter / setter
来源：http://bjv.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://vst.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://otf.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://acb.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://xvk.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://vfq.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cve.ybcxt.top

Ruby: attr_accessor :name
来源：http://rqr.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://lvc.quarkkingdee.top

[G12] 对象转字符串
来源：http://nev.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://qsa.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://zkm.yonumen.top

JS:   toString() { return this.name; }
来源：http://hdj.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://wus.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://uvd.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://atp.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://cnj.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://iad.chenlongwang.top

[G13] 判断对象类型
来源：http://gwm.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://jsn.9152youxi.cn

PHP:  $u instanceof User
来源：http://jgy.yanxiufei.cn

JS:   u instanceof User
来源：http://uer.shangyingyoupin.top

TS:   u instanceof User
来源：http://cat.fktsv.cn

Java: u instanceof User
来源：http://dcg.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kaj.cucudq.cn

Ruby: u.is_a?(User)
来源：http://rek.nwbrower.top

C#:   u is User
来源：http://twg.ehwqpu.com

[G14] 数据类 / record
来源：http://ugt.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjk.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://bja.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://fty.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://xvy.mhx1999.top

Java: record User(String name, int age) {}
来源：http://ehb.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://kgd.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kwx.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://tzi.dashuyun.cn

[G15] 枚举
来源：http://xox.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vqw.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ikj.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://icx.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ley.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://ijg.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://quw.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://qkv.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hjx.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ktf.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fxm.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://skf.yj20258888.top

JS:   Object.entries(obj)
来源：http://tzc.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://wre.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ltl.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bua.yj20258888.top

Ruby: obj.instance_variables
来源：http://hoq.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://tya.chenjidiqi.icu

================================================================================
来源：http://cwj.wangshuangyany.cn

H. 异常与错误处理
来源：http://bir.ivvv.top

================================================================================
来源：http://nys.c1oappe.top

[H01] try / catch 基础
来源：http://xjr.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://afc.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xft.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjb.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://deg.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://obj.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rbx.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tsm.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kwu.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://txb.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://dmc.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://etx.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vhr.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jtx.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://uwf.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sls.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ons.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ozw.chenzaomai.com

[H03] 主动抛出异常
来源：http://mgu.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://fon.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rvb.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://ubx.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://ggd.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zer.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hve.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kfk.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://inw.hcnkem.com

[H04] 自定义异常类型
来源：http://owu.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://meh.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rhp.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://boy.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://imx.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://ssh.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://thr.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://pnf.ivvv.top

C#:   class MyException : Exception {}
来源：http://nmy.xziqi.cn

[H05] 捕获特定类型
来源：http://xit.yj202588.top

Py:   except ValueError as e:
来源：http://gpl.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vxf.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://ikt.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://shr.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://kvy.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ybz.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://hor.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bxp.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://vkf.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://qjf.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mjx.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zls.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://poj.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wlh.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jcu.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://azm.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://xdg.quarkkingdee.top

[H07] 断言
来源：http://lnn.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://vos.nanxinkj.top

PHP:  assert($x > 0);
来源：http://lqu.andypj.xyz

JS:   console.assert(x > 0);
来源：http://szn.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://oto.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://kfi.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kbb.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://svm.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://doc.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://tkp.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://ypj.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dmb.fktsv.cn

JS:   e.message;  e.stack
来源：http://xvh.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://inq.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://van.wangdashe.top

Go:   err.Error()
来源：http://ddv.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://lum.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://hhp.havefunace.top

[H09] 带错误码的异常
来源：http://lbt.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lpj.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://deo.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://onv.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sbg.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ukw.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dtg.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ieo.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://idy.hammf.cn

[H10] 资源自动释放
来源：http://zsj.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kks.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yjq.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eun.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgn.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qux.ctjpmb.com

Go:   defer f.Close()
来源：http://gok.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://coy.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://erc.dianchejie.cn

================================================================================
来源：http://iqh.yj20258.top

I. 正则表达式
来源：http://oie.cashguo.top

================================================================================
来源：http://jtb.zhixingplan.top

[I01] 判断是否匹配
来源：http://igb.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ckm.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lsx.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://vxp.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://akq.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mvp.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://anb.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://hrq.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dni.316326.xyz

[I02] 提取所有匹配
来源：http://rtg.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://dcx.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpv.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ssd.yj202588.top

TS:   s.match(/\d+/g)
来源：http://xjr.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uct.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pek.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://roh.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://efs.cucudq.cn

[I03] 提取捕获分组
来源：http://zlo.ivvv.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://coj.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rhg.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://idf.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gly.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pvh.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bxj.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mzq.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wle.jlsjyb.cn

[I04] 正则替换
来源：http://jfx.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gpf.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jhr.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xor.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ygi.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dks.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xqn.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ajg.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pgi.zdqjudy.top

[I05] 按正则拆分
来源：http://amu.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oyg.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jex.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://iiu.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://bso.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://wds.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://npk.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gkw.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bki.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://usk.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rsb.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ntw.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tla.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dej.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://knx.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uin.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ajc.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qtv.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://hno.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ldq.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nbs.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rte.andypj.xyz

TS:   /error/gim
来源：http://gqd.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://psa.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://moe.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://otv.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://feq.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://pqf.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xel.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rim.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwr.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tbf.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lfp.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ieq.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://slv.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fnl.ctjpmb.com

================================================================================
来源：http://lmg.birdmap.top

J. 日期与时间
来源：http://cve.jiagoushi.top

================================================================================
来源：http://wiz.cqqwz.cn

[J01] 获取当前时间
来源：http://kbs.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wmz.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://meh.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://qdt.mhx1999.top

TS:   new Date();  Date.now()
来源：http://tct.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://coc.zhijiandao.cn

Go:   time.Now()
来源：http://ele.ydzc1.top

Ruby: Time.now
来源：http://mit.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgn.c1oappe.top

[J02] 格式化输出
来源：http://two.9152youxi.cn


<!-- 参考信息 -->