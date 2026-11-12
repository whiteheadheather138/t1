代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://lhn.yvedp.cn

[G07] 调用父类方法
来源：http://xnt.ppjwa.cn

Py:   super().greet()
来源：http://qxi.aibaodan.cn

PHP:  parent::greet();
来源：http://zfq.zhijiandao.cn

JS:   super.greet();
来源：http://yhh.jlsjyb.cn

TS:   super.greet();
来源：http://dxt.gogol.net.cn

Java: super.greet();
来源：http://ssi.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tob.chenjidiqi.icu

Ruby: super
来源：http://wlb.cdnleiting.top

C#:   base.Greet();
来源：http://mwb.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://ved.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rwf.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://cmv.nanxinkj.top

JS:   static f() {}
来源：http://zji.gotoacloud.top

TS:   static f(): void {}
来源：http://mhb.zhixingplan.top

Java: static void f() {}
来源：http://ven.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://squ.gaohongyu789.top

Ruby: def self.f; end
来源：http://nex.fehbvm.com

C#:   public static void F() {}
来源：http://ykt.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://vns.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://ybd.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://msr.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dcw.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://phr.yfazqb.com

Java: interface Shape { double area(); }
来源：http://tkx.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://gin.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baf.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://tfs.jinqigufen.top

[G10] 访问控制
来源：http://pvo.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://iih.shangyingyoupin.top

PHP:  public / protected / private
来源：http://ojd.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://zrn.hcnkem.com

TS:   public / protected / private
来源：http://otw.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://ffy.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yed.zhongyouzk.top

Ruby: public / protected / private
来源：http://cem.yj20258.top

C#:   public / protected / private / internal
来源：http://dwn.hnqzz.top

[G11] getter / setter
来源：http://fam.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://oap.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mwo.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://yjj.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://xrr.fktsv.cn

Java: public String getName() { return name; }
来源：http://xjl.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xwc.svipenyu.cn

Ruby: attr_accessor :name
来源：http://apt.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://aax.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://oai.yonumen.top

Py:   def __str__(self): return self.name
来源：http://cqo.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nba.yueranfly.top

JS:   toString() { return this.name; }
来源：http://jtu.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://wzw.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://usk.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xba.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://wju.meibo888.top

C#:   public override string ToString() => Name;
来源：http://frw.hcnkem.com

[G13] 判断对象类型
来源：http://kjg.guannengcc.top

Py:   isinstance(u, User)
来源：http://vpa.zdbjq.cn

PHP:  $u instanceof User
来源：http://ate.mhx1999.top

JS:   u instanceof User
来源：http://ixa.tarul.cn

TS:   u instanceof User
来源：http://yqp.0kj1m.cn

Java: u instanceof User
来源：http://bpj.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sjc.yvedp.cn

Ruby: u.is_a?(User)
来源：http://vgw.sysykeji.top

C#:   u is User
来源：http://nmx.tian-w.cn

[G14] 数据类 / record
来源：http://zun.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ulp.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://fil.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://mdg.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://gna.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://nlt.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://irf.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lxk.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://yko.gotoacloud.top

[G15] 枚举
来源：http://bmm.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wym.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dmp.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mul.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tzn.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://wsa.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hss.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://plq.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jgg.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://ijs.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://khs.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://bgu.hywenlv.cn

JS:   Object.entries(obj)
来源：http://rth.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://vgz.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ujx.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qdo.hysaishi.cn

Ruby: obj.instance_variables
来源：http://rer.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://ypd.shuidangran.top

================================================================================
来源：http://mdq.daxiang520.top

H. 异常与错误处理
来源：http://wdp.0kj1m.cn

================================================================================
来源：http://hzs.hnqzz.top

[H01] try / catch 基础
来源：http://inm.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://coa.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lvz.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://err.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ojd.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tyr.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://veu.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xrw.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tgg.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://qcg.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://sac.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://bgg.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wit.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lsd.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://tzh.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ptv.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bca.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nct.zycfv.cn

[H03] 主动抛出异常
来源：http://itp.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://idf.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lst.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://cot.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://iwp.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://haj.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hix.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wao.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lqa.jyoumei.cn

[H04] 自定义异常类型
来源：http://zha.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://adb.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://tlo.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://gwt.yueranfly.top

TS:   class MyError extends Error {}
来源：http://bdh.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://akq.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wlb.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://kjj.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://ehv.uphjek.com

[H05] 捕获特定类型
来源：http://jjx.jqgfzy.top

Py:   except ValueError as e:
来源：http://pei.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gxe.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://hgm.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://rgq.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://lxv.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mse.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://wba.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fmd.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://xkj.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://nhi.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://att.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mie.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://hch.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tlg.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ggy.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://hid.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://ows.hfpthk.cn

[H07] 断言
来源：http://adt.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://cfs.sufxvd.cn

PHP:  assert($x > 0);
来源：http://uvr.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://ofz.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://kcm.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://npq.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bxw.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://udr.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://gnx.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://wfs.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://qgu.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hwo.zdqjudy.top

JS:   e.message;  e.stack
来源：http://fmp.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mbw.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rho.wangshuangyany.cn

Go:   err.Error()
来源：http://wpr.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://uql.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://efx.0kj1m.cn

[H09] 带错误码的异常
来源：http://zww.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tpa.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gjm.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://scz.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jak.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lfz.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fpu.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://yxm.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://euz.wangshuangyany.cn

[H10] 资源自动释放
来源：http://ukf.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pko.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lrs.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oef.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sda.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wea.redwolf501.top

Go:   defer f.Close()
来源：http://qft.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://grl.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yhl.316326.xyz

================================================================================
来源：http://eow.kuanghao11.cn

I. 正则表达式
来源：http://tzw.jinqigfzy.top

================================================================================
来源：http://cwq.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://lkr.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mqd.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nwu.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://uoe.xziqi.cn

TS:   /\d+/.test(s)
来源：http://tkc.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvy.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://knf.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://drj.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ubv.meibo888.top

[I02] 提取所有匹配
来源：http://hqa.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://vgr.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eut.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://swy.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://ivj.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vld.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://swt.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://wou.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zba.havefunace.top

[I03] 提取捕获分组
来源：http://bhi.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bro.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ini.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fpw.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://knl.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tmz.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jsl.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://scs.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://swb.vehdjk.com

[I04] 正则替换
来源：http://dwv.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://huk.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vaq.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sfu.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vvh.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://hqt.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kpq.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://rcd.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tkl.xuanzx.com

[I05] 按正则拆分
来源：http://fwv.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lcn.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fzo.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://gqu.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://unp.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://yyo.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qbm.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://njq.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqm.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pup.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dsn.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://utc.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://euh.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gmq.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qvt.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kym.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rwh.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ozl.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://dbb.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nsu.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iwk.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysg.cqqwz.cn

TS:   /error/gim
来源：http://kpe.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://roe.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nxu.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://dfs.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gmp.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://eid.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jhg.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bfp.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwi.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulf.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://xoi.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vpo.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://msr.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fuo.hesvh.cn

================================================================================
来源：http://ayc.52xcode.cn

J. 日期与时间
来源：http://smy.cdnleiting.top

================================================================================
来源：http://wgs.xuanzx.com

[J01] 获取当前时间
来源：http://utd.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tam.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ufn.c1oappe.top

JS:   new Date();  Date.now()
来源：http://ewa.gzhubu.top

TS:   new Date();  Date.now()
来源：http://eud.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mlt.yj20258888.top

Go:   time.Now()
来源：http://xnt.gaohongyu789.top

Ruby: Time.now
来源：http://ofo.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aza.gzhubu.top

[J02] 格式化输出
来源：http://aex.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nuk.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tof.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrv.ivvv.top

TS:   d.toISOString()
来源：http://lxs.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gcc.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cot.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqq.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://chu.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://sub.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bcu.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://act.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://zok.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://yei.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://cgv.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tlh.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://wxa.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://brj.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://tmc.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jgg.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://omt.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uwi.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pgh.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://opw.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://irt.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tqt.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xgw.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://jwy.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://nai.gzhubu.top


<!-- 参考信息 -->