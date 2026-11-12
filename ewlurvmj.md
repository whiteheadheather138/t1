代发 wailian999

JS:   this.name = "x";
来源：http://maj.birdmap.top

TS:   name: string = "x";
来源：http://arv.vqdsnc.cn

Java: private String name;
来源：http://qph.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lnj.yonumen.top

Ruby: @name = "x"
来源：http://ywo.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://bbl.yonumen.top

[G04] 定义方法
来源：http://tle.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://msc.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bul.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://okh.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://sqq.tanke756.top

Java: String greet() { return name; }
来源：http://ljp.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ycg.tanke756.top

Ruby: def greet; @name; end
来源：http://msq.tarul.cn

C#:   public string Greet() => Name;
来源：http://osj.jlsjyb.cn

[G05] 继承
来源：http://wbl.yj20258.top

Py:   class Admin(User): pass
来源：http://hsa.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://arz.yuanzhike.top

JS:   class Admin extends User {}
来源：http://lcg.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://zee.nwbrower.top

Java: class Admin extends User {}
来源：http://qty.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://saw.ivvv.top

Ruby: class Admin < User; end
来源：http://ahl.aizwys.cn

C#:   class Admin : User {}
来源：http://yor.iojbl.cn

[G06] 重写方法
来源：http://llb.yonumen.top

Py:   def greet(self): return "admin"
来源：http://kcy.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ovk.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://fhz.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://hns.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://dqn.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://man.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://acg.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://ifq.chenlongwang.top

[G07] 调用父类方法
来源：http://xwd.pengpengdd.cyou

Py:   super().greet()
来源：http://imr.0kj1m.cn

PHP:  parent::greet();
来源：http://fgm.fengsongda.top

JS:   super.greet();
来源：http://arr.cashguo.top

TS:   super.greet();
来源：http://bze.sufxvd.cn

Java: super.greet();
来源：http://jeq.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://njh.0kj1m.cn

Ruby: super
来源：http://nxa.pengpengdd.cyou

C#:   base.Greet();
来源：http://kto.hysaishi.cn

[G08] 静态方法与属性
来源：http://pxm.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gcf.gaohongyu789.top

PHP:  public static function f() {}
来源：http://rld.jqgfzy.top

JS:   static f() {}
来源：http://nzy.hnqzz.top

TS:   static f(): void {}
来源：http://kyn.jinqigufen.top

Java: static void f() {}
来源：http://lgi.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jqx.yj20258888.top

Ruby: def self.f; end
来源：http://edf.nanxinkj.top

C#:   public static void F() {}
来源：http://jgw.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://jqf.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ump.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://kib.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pwn.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://zyh.yonumen.top

Java: interface Shape { double area(); }
来源：http://zkx.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://hpq.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqg.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://fvk.shzxlz.cn

[G10] 访问控制
来源：http://mzu.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://xen.ybcxt.top

PHP:  public / protected / private
来源：http://vpd.yonumen.top

JS:   #private 字段；其余公开
来源：http://ggr.bjfxy.top

TS:   public / protected / private
来源：http://lpr.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://kmq.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aym.smart0.xyz

Ruby: public / protected / private
来源：http://qfp.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://lpn.tanke756.top

[G11] getter / setter
来源：http://vsm.fzhhl.top

Py:   @property 与 @x.setter
来源：http://fvm.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vhv.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://nrt.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://ssx.zycfv.cn

Java: public String getName() { return name; }
来源：http://qds.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zdw.cdnleiting.top

Ruby: attr_accessor :name
来源：http://gen.wangdashe.top

C#:   public string Name { get; set; }
来源：http://zon.yj20258.top

[G12] 对象转字符串
来源：http://kxz.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://ofs.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qrk.yongpay.top

JS:   toString() { return this.name; }
来源：http://klx.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://msw.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://dbs.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://kxc.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://ndb.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://szt.jinqigufen.top

[G13] 判断对象类型
来源：http://koa.sufxvd.cn

Py:   isinstance(u, User)
来源：http://wgf.daria6918.cn

PHP:  $u instanceof User
来源：http://bpm.shanyushiyangtech.top

JS:   u instanceof User
来源：http://fpp.ctjpmb.com

TS:   u instanceof User
来源：http://iau.chenzaomai.com

Java: u instanceof User
来源：http://vss.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hky.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://epa.yangfankeji.com

C#:   u is User
来源：http://dnw.cqqwz.cn

[G14] 数据类 / record
来源：http://hyp.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vdx.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://spj.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://vny.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://dry.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://wtj.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://dpc.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjm.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://cnu.iojbl.cn

[G15] 枚举
来源：http://lor.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iec.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://czd.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ehj.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://buk.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://gil.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kdn.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://kvh.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lwl.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://yxe.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wrj.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://vdu.zycfv.cn

JS:   Object.entries(obj)
来源：http://fjt.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://fod.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zaz.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wnl.yonumen.top

Ruby: obj.instance_variables
来源：http://vlu.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://mcc.cashguo.top

================================================================================
来源：http://cpy.aibaodan.cn

H. 异常与错误处理
来源：http://tbn.jiagoushi.top

================================================================================
来源：http://nwz.fktsv.cn

[H01] try / catch 基础
来源：http://ohl.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ufu.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ntk.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yle.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fbk.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gvd.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gbo.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tqb.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ouv.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://knc.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://rfo.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://whw.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tzu.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qje.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://rfm.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yvy.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://txm.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uwm.ctjpmb.com

[H03] 主动抛出异常
来源：http://ejg.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://ppp.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tjm.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://kdd.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://egp.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nab.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mmr.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nrs.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://pwj.gogol.net.cn

[H04] 自定义异常类型
来源：http://oan.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://yix.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uls.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://jus.fktsv.cn

TS:   class MyError extends Error {}
来源：http://cqh.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://fap.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nvf.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://ubq.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://iij.guowangkeji.top

[H05] 捕获特定类型
来源：http://edu.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://lbo.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nol.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://sar.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://uxr.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://zct.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sju.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://kjp.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zvl.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://qea.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://rjh.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://cjd.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ehv.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wuc.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ptt.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mck.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://tah.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://bfq.gotoacloud.top

[H07] 断言
来源：http://zlu.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://tym.smart0.xyz

PHP:  assert($x > 0);
来源：http://kxt.yonumen.top

JS:   console.assert(x > 0);
来源：http://qrd.jianghu66.top

TS:   console.assert(x > 0);
来源：http://xbv.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://wqs.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xbv.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://szh.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://oqe.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://dlh.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://dza.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtk.andypj.xyz

JS:   e.message;  e.stack
来源：http://uob.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rvm.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kjn.cashguo.top

Go:   err.Error()
来源：http://spn.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://oue.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://boz.havefunace.top

[H09] 带错误码的异常
来源：http://frs.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjc.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wzg.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oid.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vus.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uzo.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://top.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://lpb.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ufj.hnxiangtu.top

[H10] 资源自动释放
来源：http://nbv.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mwj.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kvc.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kyy.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kro.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://atq.hongshengwenyu.top

Go:   defer f.Close()
来源：http://mzt.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rip.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipd.jyoumei.cn

================================================================================
来源：http://eid.aizwys.cn

I. 正则表达式
来源：http://nlo.zhaomingkeji.xyz

================================================================================
来源：http://vhk.shuidangran.top

[I01] 判断是否匹配
来源：http://twh.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hvf.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hkm.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://ljf.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://jwt.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ygk.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wkh.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://tvx.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fmq.gotoacloud.top

[I02] 提取所有匹配
来源：http://yjq.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://fvu.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iwo.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghn.tanke756.top

TS:   s.match(/\d+/g)
来源：http://rgv.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ewc.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tyk.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://aml.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pio.jinqigfzy.top

[I03] 提取捕获分组
来源：http://zmh.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zsx.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkg.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://etd.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pee.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pad.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rzn.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cmr.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vux.gzhubu.top

[I04] 正则替换
来源：http://yqq.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pil.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qaj.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://lxh.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cdm.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://mfs.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ptm.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://exj.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yae.chenlongwang.top

[I05] 按正则拆分
来源：http://ywc.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://meg.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tvu.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://pyp.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://hoa.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://hec.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://okz.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://ldr.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xyk.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cog.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tln.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gse.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bfx.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlu.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qrt.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qnn.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hod.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://clf.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://mfo.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jua.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cws.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xmp.gogol.net.cn

TS:   /error/gim
来源：http://ztr.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://llt.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xrd.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://aet.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vdh.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://hcd.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://srw.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bhn.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xij.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ayx.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://aye.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wlf.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nzy.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ili.xuetiantiany.cn

================================================================================
来源：http://rda.jlsjyb.cn

J. 日期与时间
来源：http://vvj.nanxinkj.top

================================================================================
来源：http://hdq.xuanzx.com

[J01] 获取当前时间
来源：http://wfc.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rig.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gva.cucudq.cn

JS:   new Date();  Date.now()
来源：http://smm.iojbl.cn

TS:   new Date();  Date.now()
来源：http://ktl.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://pjn.zhaomingkeji.xyz


<!-- 参考信息 -->