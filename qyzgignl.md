代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://vfl.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://ili.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wjt.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://cku.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://gpr.dianchejie.cn

[G07] 调用父类方法
来源：http://mbc.jinyuanbaomall.cn

Py:   super().greet()
来源：http://tdp.chenjidiqi.icu

PHP:  parent::greet();
来源：http://vkn.yongpay.top

JS:   super.greet();
来源：http://dfl.wangdashe.top

TS:   super.greet();
来源：http://hpq.xuetiantiany.cn

Java: super.greet();
来源：http://wbr.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jqp.zhaomingkeji.xyz

Ruby: super
来源：http://tur.sufxvd.cn

C#:   base.Greet();
来源：http://hfj.zdqjudy.top

[G08] 静态方法与属性
来源：http://soi.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ulm.shuidangran.top

PHP:  public static function f() {}
来源：http://mhs.ydjk.org.cn

JS:   static f() {}
来源：http://whm.fktsv.cn

TS:   static f(): void {}
来源：http://ldt.hongshengwenyu.top

Java: static void f() {}
来源：http://wxv.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://grf.cqqwz.cn

Ruby: def self.f; end
来源：http://zyx.hnxiangtu.top

C#:   public static void F() {}
来源：http://gej.52xcode.cn

[G09] 接口 / 抽象类
来源：http://tvz.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://quh.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rfz.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ima.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://ubm.tarul.cn

Java: interface Shape { double area(); }
来源：http://dyd.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://irx.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dqr.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://kwa.yj202588.top

[G10] 访问控制
来源：http://gkr.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://nfn.yj202588.top

PHP:  public / protected / private
来源：http://zyl.tian-w.cn

JS:   #private 字段；其余公开
来源：http://tuo.yuanzhike.top

TS:   public / protected / private
来源：http://fep.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://yfo.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdo.gotoacloud.top

Ruby: public / protected / private
来源：http://nwo.zdbjq.cn

C#:   public / protected / private / internal
来源：http://uxo.kuanghao11.cn

[G11] getter / setter
来源：http://usp.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://aec.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ipp.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://xqw.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://apa.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://rmf.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xph.guannengcc.top

Ruby: attr_accessor :name
来源：http://vaf.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://xhb.cucudq.cn

[G12] 对象转字符串
来源：http://vgu.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://xmb.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kxa.yueranfly.top

JS:   toString() { return this.name; }
来源：http://obu.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://bxm.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://qgg.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ekj.yvedp.cn

Ruby: def to_s; @name; end
来源：http://ycx.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://gza.yj202588.top

[G13] 判断对象类型
来源：http://zzd.yuxming.cn

Py:   isinstance(u, User)
来源：http://gzg.guowangkeji.top

PHP:  $u instanceof User
来源：http://tyc.yueranfly.top

JS:   u instanceof User
来源：http://alf.iojbl.cn

TS:   u instanceof User
来源：http://qra.chenzaomai.com

Java: u instanceof User
来源：http://fco.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gbt.gzhubu.top

Ruby: u.is_a?(User)
来源：http://iha.zhixingplan.top

C#:   u is User
来源：http://fhz.ctjpmb.com

[G14] 数据类 / record
来源：http://ddn.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fvf.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zvg.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://cjz.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://fjw.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ovu.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://zrq.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kvs.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://tij.ctjpmb.com

[G15] 枚举
来源：http://rlg.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wfw.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kiy.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aaq.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ebq.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://iiz.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxp.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://aax.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mkc.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://umr.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qba.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://bmq.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://duv.fktsv.cn

TS:   Object.entries(obj)
来源：http://sks.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://icn.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dtt.jianghu66.top

Ruby: obj.instance_variables
来源：http://zkl.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://smb.hfpthk.cn

================================================================================
来源：http://gwh.svipenyu.cn

H. 异常与错误处理
来源：http://stj.52xcode.cn

================================================================================
来源：http://iwo.316326.xyz

[H01] try / catch 基础
来源：http://tnx.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xtq.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qbz.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zvf.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dfj.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fgz.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mra.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gox.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hgm.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://ptp.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://wcd.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ioo.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wad.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://igg.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://lnf.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hab.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cdd.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://equ.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://cdn.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://ddl.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://keh.cheryme.top

JS:   throw new Error("错误信息");
来源：http://aar.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://owm.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gwv.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qos.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gmp.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://xzu.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://bpj.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://wri.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://uvo.hammf.cn

JS:   class MyError extends Error {}
来源：http://ovh.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://vfv.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://jfp.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ddo.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://pbm.redwolf501.top

C#:   class MyException : Exception {}
来源：http://ykw.zhijiandao.cn

[H05] 捕获特定类型
来源：http://ylc.zhoulong.xyz

Py:   except ValueError as e:
来源：http://sdb.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfq.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://crg.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://pke.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://ayk.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tvb.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://qep.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mqb.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://yer.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://hct.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cfx.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://psx.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://xhd.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yyl.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hbo.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://zka.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://tlc.hcnkem.com

[H07] 断言
来源：http://ree.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://cuj.yuanzhike.top

PHP:  assert($x > 0);
来源：http://eqr.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://sgj.epnwcf.com

TS:   console.assert(x > 0);
来源：http://qfc.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://vsp.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qgo.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iku.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://bvt.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://bzr.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://iec.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://twr.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://rvi.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ian.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xsp.pycfn.com

Go:   err.Error()
来源：http://rgi.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://eab.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://akb.svipenyu.cn

[H09] 带错误码的异常
来源：http://ies.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ajb.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vht.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://inn.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wwe.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ryo.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lmi.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wmm.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hvx.cdnleiting.top

[H10] 资源自动释放
来源：http://dyl.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nzc.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bsv.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pkp.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://trz.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://azt.aizwys.cn

Go:   defer f.Close()
来源：http://yox.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://roo.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cpp.hesvh.cn

================================================================================
来源：http://qta.ydzc1.top

I. 正则表达式
来源：http://eao.andypj.xyz

================================================================================
来源：http://bxs.cqqwz.cn

[I01] 判断是否匹配
来源：http://nna.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xga.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://ofw.uphjek.com

JS:   /\d+/.test(s)
来源：http://dsh.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://hxp.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jrt.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jlg.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://xth.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gsh.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://kzo.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://ili.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ltf.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://klr.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://tfd.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://opv.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://voo.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://lgv.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ned.daxiang520.top

[I03] 提取捕获分组
来源：http://tvb.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vos.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hvr.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cxb.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ppg.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ypn.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://svr.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://arz.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xxp.shzxlz.cn

[I04] 正则替换
来源：http://ome.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jyx.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gqu.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://bwm.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vus.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://fvk.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://klh.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ygp.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fqu.pengpengdd.cyou

[I05] 按正则拆分
来源：http://dcs.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pkd.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dpk.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://oiw.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://gyy.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://psl.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yif.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://umb.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pxq.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qgu.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dic.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tiv.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bey.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cud.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eps.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vba.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://muw.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jpc.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://olh.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oep.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://djp.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gzf.sjlbkw.cn

TS:   /error/gim
来源：http://wzy.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggv.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yua.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://lzb.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fcp.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://uiu.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gve.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eae.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tkn.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dhe.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qra.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fvb.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdb.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cit.hongshengwenyu.top

================================================================================
来源：http://ine.epnwcf.com

J. 日期与时间
来源：http://aud.nanxinkj.top

================================================================================
来源：http://syf.sysykeji.top

[J01] 获取当前时间
来源：http://eml.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pza.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nla.birdmap.top

JS:   new Date();  Date.now()
来源：http://hae.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://gbv.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://kop.nwbrower.top

Go:   time.Now()
来源：http://tdz.feifeiyinyue.top

Ruby: Time.now
来源：http://rso.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpq.fengsongda.top

[J02] 格式化输出
来源：http://qoi.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://isb.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rzf.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lgf.hywenlv.cn

TS:   d.toISOString()
来源：http://tsf.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oga.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xks.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ijb.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpg.andypj.xyz

[J03] 字符串解析为日期
来源：http://kvj.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://izo.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qkm.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://ywk.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://alc.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://soe.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ctu.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://dfn.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qvk.cashguo.top

[J04] 时间戳与日期互转
来源：http://mds.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://twa.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewa.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://scm.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fcq.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lfc.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jkk.jinqigfzy.top


<!-- 参考信息 -->