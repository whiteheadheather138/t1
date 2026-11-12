代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://gjj.jqgfzy.top

[G03] 实例属性
来源：http://fzu.bjfxy.top

Py:   self.name = "x"
来源：http://ypw.cucudq.cn

PHP:  public string $name = "x";
来源：http://ama.jinqigfzy.top

JS:   this.name = "x";
来源：http://myk.daria6918.cn

TS:   name: string = "x";
来源：http://qkb.pycfn.com

Java: private String name;
来源：http://bfu.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xrv.jyoumei.cn

Ruby: @name = "x"
来源：http://heq.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://ibe.316326.xyz

[G04] 定义方法
来源：http://nat.sysykeji.top

Py:   def greet(self): return self.name
来源：http://rwj.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fqy.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://vti.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://kzp.yj202588.top

Java: String greet() { return name; }
来源：http://mux.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kng.shzxlz.cn

Ruby: def greet; @name; end
来源：http://onr.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://yzg.hongshengwenyu.top

[G05] 继承
来源：http://lhi.xuanzx.com

Py:   class Admin(User): pass
来源：http://vpc.uphjek.com

PHP:  class Admin extends User {}
来源：http://hou.nwbrower.top

JS:   class Admin extends User {}
来源：http://pxt.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://fnw.sweek.top

Java: class Admin extends User {}
来源：http://crw.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mod.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://qpb.gotoacloud.top

C#:   class Admin : User {}
来源：http://sgd.svipenyu.cn

[G06] 重写方法
来源：http://izp.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://xbt.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://laf.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://vrq.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://meo.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://agk.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cab.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://wsv.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://gev.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://dvk.tian-w.cn

Py:   super().greet()
来源：http://wfv.jianghu66.top

PHP:  parent::greet();
来源：http://ttl.feifeiyinyue.top

JS:   super.greet();
来源：http://wlq.fengsongda.top

TS:   super.greet();
来源：http://xnx.kuanghao11.cn

Java: super.greet();
来源：http://ftg.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tdh.ppjwa.cn

Ruby: super
来源：http://gxg.yuanzhike.top

C#:   base.Greet();
来源：http://ici.daxiang520.top

[G08] 静态方法与属性
来源：http://svb.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bey.daria6918.cn

PHP:  public static function f() {}
来源：http://whb.hywenlv.cn

JS:   static f() {}
来源：http://mct.xuetiantiany.cn

TS:   static f(): void {}
来源：http://uah.daria6918.cn

Java: static void f() {}
来源：http://jnl.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nun.jlsjyb.cn

Ruby: def self.f; end
来源：http://hkl.yangfankeji.com

C#:   public static void F() {}
来源：http://ofw.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://ooe.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://tsp.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://usv.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ner.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://xur.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://sjs.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://qrx.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://upa.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://frf.jinghuilouyu.cn

[G10] 访问控制
来源：http://jet.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://syh.jianghu66.top

PHP:  public / protected / private
来源：http://orv.fehbvm.com

JS:   #private 字段；其余公开
来源：http://npx.quarkkingdee.top

TS:   public / protected / private
来源：http://ndp.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://foh.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://crz.yonumen.top

Ruby: public / protected / private
来源：http://ics.ehwqpu.com

C#:   public / protected / private / internal
来源：http://mfy.daria6918.cn

[G11] getter / setter
来源：http://pzv.shuidangran.top

Py:   @property 与 @x.setter
来源：http://oex.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sll.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://qks.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://uiz.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://qhb.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ego.epnwcf.com

Ruby: attr_accessor :name
来源：http://ret.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://uls.meibo888.top

[G12] 对象转字符串
来源：http://bgi.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://dsc.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jpe.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://rdj.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://xgw.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ixu.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wiz.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://wyq.yongpay.top

C#:   public override string ToString() => Name;
来源：http://ewp.yonumen.top

[G13] 判断对象类型
来源：http://sfn.ppjwa.cn

Py:   isinstance(u, User)
来源：http://ysg.sufxvd.cn

PHP:  $u instanceof User
来源：http://ywg.hongshengwenyu.top

JS:   u instanceof User
来源：http://lcv.xylfe.cn

TS:   u instanceof User
来源：http://pkv.sweek.top

Java: u instanceof User
来源：http://egq.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jbe.shuidangran.top

Ruby: u.is_a?(User)
来源：http://wer.andypj.xyz

C#:   u is User
来源：http://mbv.jqgufenzy.top

[G14] 数据类 / record
来源：http://qbs.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ydy.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://yfy.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rlk.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://ntv.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://vru.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://mlc.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwo.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://tvk.guannengcc.top

[G15] 枚举
来源：http://crg.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sng.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jea.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fsb.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wcr.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://tlz.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rkv.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://ysw.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bfd.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://avn.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sxj.ivvv.top

PHP:  get_object_vars($obj);
来源：http://ddm.fzhhl.top

JS:   Object.entries(obj)
来源：http://wjy.dianchejie.cn

TS:   Object.entries(obj)
来源：http://zpk.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vgp.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hpf.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://yxb.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://whe.shangyingyoupin.top

================================================================================
来源：http://mem.yuanzhike.top

H. 异常与错误处理
来源：http://iqt.shangyingyoupin.top

================================================================================
来源：http://xtr.sxryk.cn

[H01] try / catch 基础
来源：http://fff.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qrg.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jty.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jom.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zpk.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yfx.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oif.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ezo.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iub.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://llb.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://pis.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nhr.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://glt.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ikn.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://sfq.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rbb.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ust.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhv.hammf.cn

[H03] 主动抛出异常
来源：http://llt.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://xsy.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ajk.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://myj.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://can.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rbo.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zlq.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://syc.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://izh.shuidangran.top

[H04] 自定义异常类型
来源：http://cru.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://sog.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zba.sysykeji.top

JS:   class MyError extends Error {}
来源：http://pbj.yvedp.cn

TS:   class MyError extends Error {}
来源：http://rxi.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://kff.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ynm.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://fuu.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://hcq.yvedp.cn

[H05] 捕获特定类型
来源：http://jhk.cqqwz.cn

Py:   except ValueError as e:
来源：http://lgd.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qok.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://fgm.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gri.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://mzu.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gub.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://ieo.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vgm.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://fue.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://wyu.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://lxd.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eok.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://iwr.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://knz.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cmz.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://npn.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://fzo.svipenyu.cn

[H07] 断言
来源：http://jdr.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://jcx.0kj1m.cn

PHP:  assert($x > 0);
来源：http://lmj.yj20258888.top

JS:   console.assert(x > 0);
来源：http://rcf.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://crs.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://anz.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://isg.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://mtt.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://dty.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://msh.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://grz.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ewc.xinyue.icu

JS:   e.message;  e.stack
来源：http://vmw.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kat.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://uiw.chenzaomai.com

Go:   err.Error()
来源：http://akr.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://jau.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://khl.shuidangran.top

[H09] 带错误码的异常
来源：http://rtp.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yzd.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kcb.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xps.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nid.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wlo.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jmk.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bfi.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xwu.bbcook.cn

[H10] 资源自动释放
来源：http://bwu.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bkw.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://faf.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ydt.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tnb.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bor.chenlongwang.top

Go:   defer f.Close()
来源：http://ivh.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://koh.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uwk.cucudq.cn

================================================================================
来源：http://hik.vehdjk.com

I. 正则表达式
来源：http://rfw.yuxming.cn

================================================================================
来源：http://zey.dashuyun.cn

[I01] 判断是否匹配
来源：http://bns.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eoz.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yax.birdmap.top

JS:   /\d+/.test(s)
来源：http://drf.pycfn.com

TS:   /\d+/.test(s)
来源：http://wtt.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ela.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gfv.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://sdu.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qey.yj20258.top

[I02] 提取所有匹配
来源：http://oqp.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://iut.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gcy.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://keo.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://gfh.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ofn.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rcr.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://plp.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ckz.fengsongda.top

[I03] 提取捕获分组
来源：http://xhr.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://atn.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lls.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yjg.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://myx.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vim.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ome.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fcg.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jei.ydzc1.top

[I04] 正则替换
来源：http://wsc.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wlk.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjr.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://brv.yongpay.top

TS:   s.replace(/\d+/g, "#")
来源：http://awz.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://mhs.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ycj.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oww.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gsr.andypj.xyz

[I05] 按正则拆分
来源：http://pcp.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://atp.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uvh.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://yqo.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://quj.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://xhq.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uct.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://acb.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bsq.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nwf.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vow.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ijg.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khd.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvd.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pya.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hhv.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bqa.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bko.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://rtw.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bry.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kme.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sdf.aizwys.cn

TS:   /error/gim
来源：http://lqc.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://thv.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tqj.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://ebf.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mbz.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://nss.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://txg.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://osw.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://djo.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blh.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tla.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uec.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ljc.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lcn.smart0.xyz

================================================================================
来源：http://vtu.ivvv.top

J. 日期与时间
来源：http://lsu.daxiang520.top

================================================================================
来源：http://cqg.zhongyouzk.top

[J01] 获取当前时间
来源：http://zbs.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zxj.yj20258.top


<!-- 参考信息 -->