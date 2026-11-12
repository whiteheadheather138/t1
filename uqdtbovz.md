代发 wailian999

JS:   super.greet();
来源：http://ymp.chenlongwang.top

TS:   super.greet();
来源：http://fnh.sjlbkw.cn

Java: super.greet();
来源：http://dxj.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gft.shzxlz.cn

Ruby: super
来源：http://tdg.zhixingplan.top

C#:   base.Greet();
来源：http://fpz.ybcxt.top

[G08] 静态方法与属性
来源：http://efx.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kyn.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://ewf.sysykeji.top

JS:   static f() {}
来源：http://vol.guowangkeji.top

TS:   static f(): void {}
来源：http://loq.yongpay.top

Java: static void f() {}
来源：http://cys.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dwx.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://plh.ehwqpu.com

C#:   public static void F() {}
来源：http://opd.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://cjc.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ntc.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://lhm.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vau.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://gsv.havefunace.top

Java: interface Shape { double area(); }
来源：http://wui.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://dhs.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wln.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://nvm.ydzc1.top

[G10] 访问控制
来源：http://sri.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://xjp.jianghu66.top

PHP:  public / protected / private
来源：http://czr.mhx1999.top

JS:   #private 字段；其余公开
来源：http://spu.ehwqpu.com

TS:   public / protected / private
来源：http://qmo.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://xsc.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://ahz.sjlbkw.cn

Ruby: public / protected / private
来源：http://kgn.0kj1m.cn

C#:   public / protected / private / internal
来源：http://oav.iojbl.cn

[G11] getter / setter
来源：http://lko.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://ubw.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bzz.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://tjh.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://thi.guannengcc.top

Java: public String getName() { return name; }
来源：http://gdz.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://olm.redwolf501.top

Ruby: attr_accessor :name
来源：http://yed.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://wkm.0kj1m.cn

[G12] 对象转字符串
来源：http://huy.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://tne.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfr.birdmap.top

JS:   toString() { return this.name; }
来源：http://ppn.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://slz.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://zng.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wue.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://woe.havefunace.top

C#:   public override string ToString() => Name;
来源：http://alh.yanxiufei.cn

[G13] 判断对象类型
来源：http://cpk.zdqjudy.top

Py:   isinstance(u, User)
来源：http://xza.jinqigufen.top

PHP:  $u instanceof User
来源：http://agi.shzxlz.cn

JS:   u instanceof User
来源：http://vdw.feifeiyinyue.top

TS:   u instanceof User
来源：http://ubm.jiagoushi.top

Java: u instanceof User
来源：http://iju.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqk.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://iku.birdmap.top

C#:   u is User
来源：http://eom.kuanghao11.cn

[G14] 数据类 / record
来源：http://oqb.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ord.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://qrc.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://fjp.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://rww.ybcxt.top

Java: record User(String name, int age) {}
来源：http://tzf.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://qca.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://itx.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://tay.daxiang520.top

[G15] 枚举
来源：http://ffb.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tqz.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vov.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mnh.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pjz.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://caw.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://njz.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://dah.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pke.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://luk.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aqn.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://odp.yfazqb.com

JS:   Object.entries(obj)
来源：http://ijm.yangfankeji.com

TS:   Object.entries(obj)
来源：http://sdt.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nuy.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vzq.gotoacloud.top

Ruby: obj.instance_variables
来源：http://oov.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://eod.meibo888.top

================================================================================
来源：http://kii.zhongyouzk.top

H. 异常与错误处理
来源：http://fwy.yonumen.top

================================================================================
来源：http://xkj.wangdashe.top

[H01] try / catch 基础
来源：http://frn.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qne.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://odg.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fiv.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pvn.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dll.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nsg.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wgr.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lqg.ivvv.top

[H02] finally / ensure 收尾
来源：http://clq.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://abz.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kva.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jdf.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ism.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yvu.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zde.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aej.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iag.jqgufenzy.top

[H03] 主动抛出异常
来源：http://atp.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://qdr.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nik.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://dav.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://dpn.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qpw.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://haa.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xwz.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://yxx.sxryk.cn

[H04] 自定义异常类型
来源：http://kbl.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://suj.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://euv.redwolf501.top

JS:   class MyError extends Error {}
来源：http://cqm.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://cal.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://xyn.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cwk.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://ulo.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://anf.zhijiandao.cn

[H05] 捕获特定类型
来源：http://yug.tian-w.cn

Py:   except ValueError as e:
来源：http://nbk.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wfy.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://hzv.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://zuo.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://qxf.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yvb.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://fho.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lit.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://gzr.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://rlf.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://xdi.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://msk.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://sqx.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vic.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hkx.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://hni.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://rhb.sxryk.cn

[H07] 断言
来源：http://sfe.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://qui.chenzaomai.com

PHP:  assert($x > 0);
来源：http://tsk.xziqi.cn

JS:   console.assert(x > 0);
来源：http://lyx.uphjek.com

TS:   console.assert(x > 0);
来源：http://qqk.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://uzq.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jux.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://ohd.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://ama.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://gwc.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://amn.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qkz.fengsongda.top

JS:   e.message;  e.stack
来源：http://jai.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bbm.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ltn.zhongyouzk.top

Go:   err.Error()
来源：http://hmv.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://koo.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://rqi.zhixingplan.top

[H09] 带错误码的异常
来源：http://czn.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mti.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wyx.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptt.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://imv.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jjd.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqi.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iic.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aui.fengsongda.top

[H10] 资源自动释放
来源：http://zeq.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://web.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://brm.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hem.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ers.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qtk.tian-w.cn

Go:   defer f.Close()
来源：http://srl.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iic.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://odd.ywan-chungtsiang.top

================================================================================
来源：http://xpr.yueranfly.top

I. 正则表达式
来源：http://ddo.yangfankeji.com

================================================================================
来源：http://bqx.cqqwz.cn

[I01] 判断是否匹配
来源：http://nhk.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rbb.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://nbj.havefunace.top

JS:   /\d+/.test(s)
来源：http://oqa.cucudq.cn

TS:   /\d+/.test(s)
来源：http://ivn.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://llw.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qbd.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://ifl.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://whl.iojbl.cn

[I02] 提取所有匹配
来源：http://kny.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://ajc.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hlx.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezp.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://rvi.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://akd.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wak.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://nuo.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://frn.zhijiandao.cn

[I03] 提取捕获分组
来源：http://tos.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://scd.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bsl.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fee.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lnm.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ooq.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vni.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hxt.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sme.ywan-chungtsiang.top

[I04] 正则替换
来源：http://avi.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oxk.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xzq.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://kas.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tkc.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://jro.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fzm.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uhu.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gpw.feifeiyinyue.top

[I05] 按正则拆分
来源：http://ret.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://szc.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ubo.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://tjy.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://njg.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://ydc.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jes.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://wjc.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nyj.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fvz.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gmk.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zhy.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbt.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yca.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xiz.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nrf.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vdy.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tkp.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://hze.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pac.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zac.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dqh.pycfn.com

TS:   /error/gim
来源：http://hit.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ndo.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgk.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://iis.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jxt.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://nnh.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ply.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jtz.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ipc.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vej.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://goi.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eaw.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sfe.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eyx.zhoulong.xyz

================================================================================
来源：http://sev.ywan-chungtsiang.top

J. 日期与时间
来源：http://lov.yfazqb.com

================================================================================
来源：http://low.xziqi.cn

[J01] 获取当前时间
来源：http://uer.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yvh.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iso.tian-w.cn

JS:   new Date();  Date.now()
来源：http://gnb.shuidangran.top

TS:   new Date();  Date.now()
来源：http://foq.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bms.bjfxy.top

Go:   time.Now()
来源：http://ksc.shzxlz.cn

Ruby: Time.now
来源：http://qtz.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yqq.gogol.net.cn

[J02] 格式化输出
来源：http://vsl.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrn.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dif.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zjf.hysaishi.cn

TS:   d.toISOString()
来源：http://lgc.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eov.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cho.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gpc.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kee.sufxvd.cn

[J03] 字符串解析为日期
来源：http://dup.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tcc.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://raz.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://gzl.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://pnm.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://drh.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vtn.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://nam.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xjt.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://ftw.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://frh.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zcb.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tmv.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ffu.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eaq.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pcf.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oam.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rdn.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://dwm.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://jvx.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ise.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajj.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nnv.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://rjf.iojbl.cn


<!-- 参考信息 -->