代发 wailian999

JS:   this.name = "x";
来源：http://czj.0kj1m.cn

TS:   name: string = "x";
来源：http://oqw.yongpay.top

Java: private String name;
来源：http://glf.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zwu.fzhhl.top

Ruby: @name = "x"
来源：http://fug.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://fpv.yongpay.top

[G04] 定义方法
来源：http://aex.fehbvm.com

Py:   def greet(self): return self.name
来源：http://dnm.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dza.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://fmj.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://uun.yfazqb.com

Java: String greet() { return name; }
来源：http://ihr.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rvh.svipenyu.cn

Ruby: def greet; @name; end
来源：http://hqj.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://uqz.pycfn.com

[G05] 继承
来源：http://cqk.ctjpmb.com

Py:   class Admin(User): pass
来源：http://hzg.fktsv.cn

PHP:  class Admin extends User {}
来源：http://wdk.svipenyu.cn

JS:   class Admin extends User {}
来源：http://uqj.wangdashe.top

TS:   class Admin extends User {}
来源：http://nbd.zdqjudy.top

Java: class Admin extends User {}
来源：http://jtw.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ypb.0kj1m.cn

Ruby: class Admin < User; end
来源：http://myn.yj202588.top

C#:   class Admin : User {}
来源：http://ext.vqdsnc.cn

[G06] 重写方法
来源：http://oym.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://ssm.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kbu.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://uhr.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://apw.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://aqg.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vgs.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://cgr.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://sxc.aizwys.cn

[G07] 调用父类方法
来源：http://jkp.andypj.xyz

Py:   super().greet()
来源：http://uur.tian-w.cn

PHP:  parent::greet();
来源：http://nbk.zhengqikj.top

JS:   super.greet();
来源：http://yxd.zhijiandao.cn

TS:   super.greet();
来源：http://luj.epnwcf.com

Java: super.greet();
来源：http://uba.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpa.ydzc1.top

Ruby: super
来源：http://kgy.hfpthk.cn

C#:   base.Greet();
来源：http://zxd.jqgufenzy.top

[G08] 静态方法与属性
来源：http://hno.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kbt.yanxiufei.cn

PHP:  public static function f() {}
来源：http://amy.vehdjk.com

JS:   static f() {}
来源：http://noa.haohaochexian.top

TS:   static f(): void {}
来源：http://cvi.sufxvd.cn

Java: static void f() {}
来源：http://rja.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://knm.vqdsnc.cn

Ruby: def self.f; end
来源：http://eot.52xcode.cn

C#:   public static void F() {}
来源：http://tok.c1oappe.top

[G09] 接口 / 抽象类
来源：http://zlo.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://hpc.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cyz.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fmk.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://oec.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://qjb.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://oag.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zkc.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://cwx.nanxuanxn.top

[G10] 访问控制
来源：http://bvz.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://opi.svipenyu.cn

PHP:  public / protected / private
来源：http://beu.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://sbj.dashuyun.cn

TS:   public / protected / private
来源：http://fkc.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://ghm.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jfm.birdmap.top

Ruby: public / protected / private
来源：http://vbk.sweek.top

C#:   public / protected / private / internal
来源：http://ger.fehbvm.com

[G11] getter / setter
来源：http://yee.xuanzx.com

Py:   @property 与 @x.setter
来源：http://esu.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xrz.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://hta.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://hji.zycfv.cn

Java: public String getName() { return name; }
来源：http://bcp.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bja.cheryme.top

Ruby: attr_accessor :name
来源：http://uck.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://wyz.shuidangran.top

[G12] 对象转字符串
来源：http://iys.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://avd.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cwq.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://zyl.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://bhv.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://dum.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://ach.jianghu66.top

Ruby: def to_s; @name; end
来源：http://mhp.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://zxt.yvedp.cn

[G13] 判断对象类型
来源：http://lzg.gzhubu.top

Py:   isinstance(u, User)
来源：http://xfp.gogol.net.cn

PHP:  $u instanceof User
来源：http://nlh.svipenyu.cn

JS:   u instanceof User
来源：http://czq.zhongyouzk.top

TS:   u instanceof User
来源：http://bgs.ppjwa.cn

Java: u instanceof User
来源：http://pdg.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dkd.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://edb.tanke756.top

C#:   u is User
来源：http://eqp.chenjidiqi.icu

[G14] 数据类 / record
来源：http://tnw.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xdf.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://zbp.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cxl.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://xet.xziqi.cn

Java: record User(String name, int age) {}
来源：http://xxb.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://oyc.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://otv.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://ujg.guowangkeji.top

[G15] 枚举
来源：http://acq.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mcm.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mmp.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yro.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mnx.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://yal.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xov.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://yiz.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bxe.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://yry.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://scv.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://wfe.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://aal.havefunace.top

TS:   Object.entries(obj)
来源：http://svf.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xor.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://evn.hammf.cn

Ruby: obj.instance_variables
来源：http://cbk.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://ymu.zdbjq.cn

================================================================================
来源：http://wwo.cashguo.top

H. 异常与错误处理
来源：http://hyy.wangdashe.top

================================================================================
来源：http://xmj.xuanzx.com

[H01] try / catch 基础
来源：http://owt.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mtg.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dmz.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fzk.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nfd.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mqe.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ipa.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ptj.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bwl.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://uxt.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pog.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uuy.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fki.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xbm.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://gxc.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bqg.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gah.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://enb.316326.xyz

[H03] 主动抛出异常
来源：http://mhw.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://tyx.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wfv.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://kwf.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://ifs.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://blx.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hnu.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gca.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lah.gzhubu.top

[H04] 自定义异常类型
来源：http://fdr.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://mun.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ush.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://lxt.hcnkem.com

TS:   class MyError extends Error {}
来源：http://qeg.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://rsx.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tap.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://ghd.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://xoz.zhixingplan.top

[H05] 捕获特定类型
来源：http://ips.yanxiufei.cn

Py:   except ValueError as e:
来源：http://uji.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vaz.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://qeh.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://ely.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://yrw.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmt.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://cxg.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sdm.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://bqd.redwolf501.top

Py:   value = d.get("k") or default
来源：http://lud.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://kpa.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://vkp.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://elf.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bfm.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rfv.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://zlp.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://yeg.hammf.cn

[H07] 断言
来源：http://ikx.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://rvi.xylfe.cn

PHP:  assert($x > 0);
来源：http://sil.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://bkc.yuxming.cn

TS:   console.assert(x > 0);
来源：http://kxk.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://nhv.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bqg.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://bsn.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://ipg.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://lfm.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://stv.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tnv.52xcode.cn

JS:   e.message;  e.stack
来源：http://kuv.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qzv.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://znu.jinqigufen.top

Go:   err.Error()
来源：http://opp.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://ska.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://oug.aibaodan.cn

[H09] 带错误码的异常
来源：http://kfh.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rjm.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hrm.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kao.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iih.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yeb.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xdo.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://lmp.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tqc.wangshuangyany.cn

[H10] 资源自动释放
来源：http://qlz.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gyr.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oao.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oet.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hhv.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://abg.tarul.cn

Go:   defer f.Close()
来源：http://baw.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tjf.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zwg.yangfankeji.com

================================================================================
来源：http://vhz.jyoumei.cn

I. 正则表达式
来源：http://aid.cqqwz.cn

================================================================================
来源：http://uly.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://ihh.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nms.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zbo.fengsongda.top

JS:   /\d+/.test(s)
来源：http://wtu.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://qqx.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://crh.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rxe.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://zys.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eph.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://aek.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://fcv.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ppa.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://grm.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://iwg.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pyv.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vcy.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://ioq.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cfl.tarul.cn

[I03] 提取捕获分组
来源：http://qep.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nxu.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uob.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yur.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oin.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jll.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ibe.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pyk.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bbq.chenzaomai.com

[I04] 正则替换
来源：http://lja.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ypu.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tcc.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://jsu.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ten.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://pls.tian-w.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ovb.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pae.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iyh.cdnleiting.top

[I05] 按正则拆分
来源：http://mjp.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kju.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qrj.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ysq.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://vvz.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://wzf.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sgh.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://jni.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hmv.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://drv.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tko.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nml.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zkd.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://luf.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tnn.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fel.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vve.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dwl.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://qaa.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aff.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oyy.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wpi.shangyingyoupin.top

TS:   /error/gim
来源：http://eaj.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tiw.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxd.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://wql.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yun.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://kpg.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cxg.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://arm.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rwj.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpl.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dbv.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sjj.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zjp.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://anb.chenzaomai.com

================================================================================
来源：http://dtc.guannengcc.top

J. 日期与时间
来源：http://oiq.jinyuanbaomall.cn

================================================================================
来源：http://qao.dianchejie.cn

[J01] 获取当前时间
来源：http://frh.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://doe.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://egi.ydzc1.top

JS:   new Date();  Date.now()
来源：http://yhk.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://wyu.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vhy.ydjk.org.cn


<!-- 参考信息 -->