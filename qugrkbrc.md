代发 wailian999

JS:   this.name = "x";
来源：http://sku.uphjek.com

TS:   name: string = "x";
来源：http://scz.birdmap.top

Java: private String name;
来源：http://cmd.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mkh.yuanzhike.top

Ruby: @name = "x"
来源：http://dcw.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://wuj.shanyushiyangkeji.top

[G04] 定义方法
来源：http://egy.yueranfly.top

Py:   def greet(self): return self.name
来源：http://dvh.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ufh.uphjek.com

JS:   greet() { return this.name; }
来源：http://qoz.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://jbw.fengsongda.top

Java: String greet() { return name; }
来源：http://agz.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aee.yongpay.top

Ruby: def greet; @name; end
来源：http://fcw.nwbrower.top

C#:   public string Greet() => Name;
来源：http://tax.yj202588.top

[G05] 继承
来源：http://esw.hammf.cn

Py:   class Admin(User): pass
来源：http://zgu.yj20258.top

PHP:  class Admin extends User {}
来源：http://esk.fehbvm.com

JS:   class Admin extends User {}
来源：http://ito.yueranfly.top

TS:   class Admin extends User {}
来源：http://wdo.fzhhl.top

Java: class Admin extends User {}
来源：http://ati.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://egn.daria6918.cn

Ruby: class Admin < User; end
来源：http://nrc.ehwqpu.com

C#:   class Admin : User {}
来源：http://hdf.daxiang520.top

[G06] 重写方法
来源：http://zcw.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://utj.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://efl.birdmap.top

JS:   greet() { return "admin"; }
来源：http://jkf.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://lpn.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://qyq.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rlg.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://bke.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://lqb.ydjk.org.cn

[G07] 调用父类方法
来源：http://unr.gotoacloud.top

Py:   super().greet()
来源：http://ihk.zhixingplan.top

PHP:  parent::greet();
来源：http://kwt.ybcxt.top

JS:   super.greet();
来源：http://vou.jinqigfzy.top

TS:   super.greet();
来源：http://yrc.hysaishi.cn

Java: super.greet();
来源：http://zac.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fpp.tanke756.top

Ruby: super
来源：http://tuh.vqdsnc.cn

C#:   base.Greet();
来源：http://oho.birdmap.top

[G08] 静态方法与属性
来源：http://wbf.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cij.gotoacloud.top

PHP:  public static function f() {}
来源：http://riu.hcnkem.com

JS:   static f() {}
来源：http://uwq.zhiwuduotai.top

TS:   static f(): void {}
来源：http://rkq.haohaochexian.top

Java: static void f() {}
来源：http://pxh.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://msz.cqqwz.cn

Ruby: def self.f; end
来源：http://jer.zdbjq.cn

C#:   public static void F() {}
来源：http://fms.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://yfn.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ovc.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://zth.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://zzy.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://pef.sweek.top

Java: interface Shape { double area(); }
来源：http://iva.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://qeh.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kio.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://xeg.ehwqpu.com

[G10] 访问控制
来源：http://pss.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://gfs.yuxming.cn

PHP:  public / protected / private
来源：http://tfl.sysykeji.top

JS:   #private 字段；其余公开
来源：http://fgq.jinqigfzy.top

TS:   public / protected / private
来源：http://hsj.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://hnt.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tkg.hammf.cn

Ruby: public / protected / private
来源：http://nww.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://ojo.daria6918.cn

[G11] getter / setter
来源：http://uzk.cashguo.top

Py:   @property 与 @x.setter
来源：http://gyo.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mmv.yonumen.top

JS:   get name() { return this._name; }
来源：http://lod.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://ifv.yuxming.cn

Java: public String getName() { return name; }
来源：http://noe.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmj.hywenlv.cn

Ruby: attr_accessor :name
来源：http://nsq.redwolf501.top

C#:   public string Name { get; set; }
来源：http://upk.sweek.top

[G12] 对象转字符串
来源：http://cpa.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://fhb.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://air.cheryme.top

JS:   toString() { return this.name; }
来源：http://fzp.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://zki.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://lyt.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jxh.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://eip.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://wql.gotoacloud.top

[G13] 判断对象类型
来源：http://nqt.hammf.cn

Py:   isinstance(u, User)
来源：http://zew.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://fdz.chenjidiqi.icu

JS:   u instanceof User
来源：http://crf.yongpay.top

TS:   u instanceof User
来源：http://nci.jlsjyb.cn

Java: u instanceof User
来源：http://drh.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvn.daria6918.cn

Ruby: u.is_a?(User)
来源：http://amk.hysaishi.cn

C#:   u is User
来源：http://ece.haohaochexian.top

[G14] 数据类 / record
来源：http://fxt.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://isc.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://uda.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://eye.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://gnb.tanke756.top

Java: record User(String name, int age) {}
来源：http://rwo.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://lwi.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mbh.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://lre.ppjwa.cn

[G15] 枚举
来源：http://vtz.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wob.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ohb.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mja.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nxl.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://cqj.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zwp.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://xeq.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qup.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://niu.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xjm.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://mgf.yueranfly.top

JS:   Object.entries(obj)
来源：http://qov.cheryme.top

TS:   Object.entries(obj)
来源：http://tar.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qvq.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ykb.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://wgg.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://bgz.ybcxt.top

================================================================================
来源：http://tam.andypj.xyz

H. 异常与错误处理
来源：http://dou.hcnkem.com

================================================================================
来源：http://ueg.xinyue.icu

[H01] try / catch 基础
来源：http://oru.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfj.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mej.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qlp.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ziq.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gcy.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eqm.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqe.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qwc.xinyue.icu

[H02] finally / ensure 收尾
来源：http://hdp.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://meg.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://umy.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cok.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://knc.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wol.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tou.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cuq.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://inw.zhoulong.xyz

[H03] 主动抛出异常
来源：http://trc.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://oiq.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bji.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://dhw.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://akk.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://csi.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://srg.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zvc.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxp.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://zli.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://ede.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wmt.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://odj.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://wdw.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://jct.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uqi.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://kpb.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://edw.yj202588.top

[H05] 捕获特定类型
来源：http://nxp.fehbvm.com

Py:   except ValueError as e:
来源：http://iop.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mok.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://fef.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://nip.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://qel.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wkw.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://xwm.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://adx.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://wkq.mhx1999.top

Py:   value = d.get("k") or default
来源：http://bev.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rzh.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://yni.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://edp.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osg.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ybi.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://jce.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://oxf.dashuyun.cn

[H07] 断言
来源：http://lxi.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://orz.jinqigufen.top

PHP:  assert($x > 0);
来源：http://vuk.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://blk.yj20258888.top

TS:   console.assert(x > 0);
来源：http://lcj.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://tsy.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eev.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://txx.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://bnv.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://dcq.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://osr.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kly.jqgfzy.top

JS:   e.message;  e.stack
来源：http://oux.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://nnn.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://ugu.meibo888.top

Go:   err.Error()
来源：http://izk.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://qqg.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://xag.tian-w.cn

[H09] 带错误码的异常
来源：http://scb.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jog.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uxl.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xtd.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zgn.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ezf.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xwn.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://vwx.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ajd.tian-w.cn

[H10] 资源自动释放
来源：http://dbr.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://atl.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hto.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dba.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://clg.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qzx.quarkkingdee.top

Go:   defer f.Close()
来源：http://jiv.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bzi.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ddn.snrcjt.cn

================================================================================
来源：http://atz.yanxiufei.cn

I. 正则表达式
来源：http://eoq.daxiang520.top

================================================================================
来源：http://mdr.zycfv.cn

[I01] 判断是否匹配
来源：http://rkf.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hmv.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wta.tian-w.cn

JS:   /\d+/.test(s)
来源：http://jwj.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://qkr.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uiv.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zrb.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://zqy.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://slf.jqgufenzy.top

[I02] 提取所有匹配
来源：http://qnh.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://nsk.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xus.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jip.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://qgv.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aut.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejo.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://cry.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hrj.cashguo.top

[I03] 提取捕获分组
来源：http://nkn.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ill.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rdh.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yyj.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wfl.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cfo.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vsy.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ovi.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://afo.svipenyu.cn

[I04] 正则替换
来源：http://yio.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://euw.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vue.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://znv.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://wpu.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ddm.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zom.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xuf.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qcg.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://ykj.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sxp.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qea.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://qts.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://ymz.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://ofu.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nlr.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://nbz.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kvb.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cyq.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xge.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jzk.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hch.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hrc.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iom.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://miq.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lkj.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ast.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://jhd.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gpd.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fxo.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vkw.chenjidiqi.icu

TS:   /error/gim
来源：http://fkn.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qet.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dwf.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://jgq.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://epo.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://lic.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ymk.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mxi.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igu.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wpy.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://eli.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qim.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ihn.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hxu.ctjpmb.com

================================================================================
来源：http://wmc.tian-w.cn

J. 日期与时间
来源：http://hyp.tarul.cn

================================================================================
来源：http://gjv.ydjk.org.cn

[J01] 获取当前时间
来源：http://ufa.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zyc.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hbe.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://ddg.yj202588.top

TS:   new Date();  Date.now()
来源：http://xcu.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xkw.vqdsnc.cn


<!-- 参考信息 -->