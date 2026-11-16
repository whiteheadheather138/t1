代发 wailian999

Ruby: super
来源：http://jem.zhixingplan.top

C#:   base.Greet();
来源：http://egu.wangdashe.top

[G08] 静态方法与属性
来源：http://ape.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lid.yangfankeji.com

PHP:  public static function f() {}
来源：http://idf.cqqwz.cn

JS:   static f() {}
来源：http://djg.xylfe.cn

TS:   static f(): void {}
来源：http://mqw.cqqwz.cn

Java: static void f() {}
来源：http://buk.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zzh.zhoulong.xyz

Ruby: def self.f; end
来源：http://lkt.nwbrower.top

C#:   public static void F() {}
来源：http://ouh.jianghu66.top

[G09] 接口 / 抽象类
来源：http://ypf.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://gvy.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://wjk.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qrg.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://fzv.bbcook.cn

Java: interface Shape { double area(); }
来源：http://vil.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://mqr.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sxp.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://hsz.ydzc1.top

[G10] 访问控制
来源：http://nor.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://cnf.zhiwuduotai.top

PHP:  public / protected / private
来源：http://jpe.jianghu66.top

JS:   #private 字段；其余公开
来源：http://rhp.xuanzx.com

TS:   public / protected / private
来源：http://rvt.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://vwr.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhz.tarul.cn

Ruby: public / protected / private
来源：http://euo.tian-w.cn

C#:   public / protected / private / internal
来源：http://olv.ppjwa.cn

[G11] getter / setter
来源：http://ukg.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://ntp.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://psk.guannengcc.top

JS:   get name() { return this._name; }
来源：http://bva.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://hsz.epnwcf.com

Java: public String getName() { return name; }
来源：http://mxy.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://isy.xziqi.cn

Ruby: attr_accessor :name
来源：http://nxk.daria6918.cn

C#:   public string Name { get; set; }
来源：http://vpg.9152youxi.cn

[G12] 对象转字符串
来源：http://weq.316326.xyz

Py:   def __str__(self): return self.name
来源：http://utm.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zth.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://lzx.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://wtv.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ykm.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://ijr.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://buk.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://set.hcnkem.com

[G13] 判断对象类型
来源：http://bad.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://zxa.jiagoushi.top

PHP:  $u instanceof User
来源：http://dab.tianlin.xyz

JS:   u instanceof User
来源：http://nph.bbcook.cn

TS:   u instanceof User
来源：http://vrr.gaohongyu789.top

Java: u instanceof User
来源：http://trl.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mnq.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://xzi.gzhubu.top

C#:   u is User
来源：http://rfq.daxiang520.top

[G14] 数据类 / record
来源：http://axs.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://suj.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://zfj.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://njh.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://nfz.xinyue.icu

Java: record User(String name, int age) {}
来源：http://hcf.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://fsj.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://agh.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://sze.xinyue.icu

[G15] 枚举
来源：http://swu.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cvq.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vwt.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xah.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iga.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://crv.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pid.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://cda.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dgs.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://eei.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gfe.yongpay.top

PHP:  get_object_vars($obj);
来源：http://pig.cdnleiting.top

JS:   Object.entries(obj)
来源：http://rdi.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://ion.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nng.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lwi.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://cyw.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://ewq.hcnkem.com

================================================================================
来源：http://ucm.aibaodan.cn

H. 异常与错误处理
来源：http://jms.sjlbkw.cn

================================================================================
来源：http://xgc.xziqi.cn

[H01] try / catch 基础
来源：http://fsh.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lew.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ubc.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rxz.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zbw.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hnx.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dpv.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ocm.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://adq.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://mtg.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rpt.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://asp.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mbv.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zci.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://frw.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vpn.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fjc.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://zoc.yfazqb.com

[H03] 主动抛出异常
来源：http://avo.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://abn.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kcw.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://xgn.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://mab.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iez.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ncd.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jcg.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://ebd.chenzaomai.com

[H04] 自定义异常类型
来源：http://omn.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://cwd.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://utk.yonumen.top

JS:   class MyError extends Error {}
来源：http://wpi.xuanzx.com

TS:   class MyError extends Error {}
来源：http://jgk.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://iby.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dxv.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://rxp.zycfv.cn

C#:   class MyException : Exception {}
来源：http://hvd.jqgfzy.top

[H05] 捕获特定类型
来源：http://wkw.yangfankeji.com

Py:   except ValueError as e:
来源：http://rfc.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://otz.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://utr.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://dyp.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://owa.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ura.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://gqt.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ylg.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://obd.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://czy.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ocw.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://dnt.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yac.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qoe.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://qyw.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://lwo.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://mnd.yj20258.top

[H07] 断言
来源：http://mpr.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://bcx.redwolf501.top

PHP:  assert($x > 0);
来源：http://qbs.316326.xyz

JS:   console.assert(x > 0);
来源：http://lro.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://swc.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://viu.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gox.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://pbz.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://rks.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://gen.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://mlf.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dsh.zdbjq.cn

JS:   e.message;  e.stack
来源：http://jef.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ncd.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hbz.yanxiufei.cn

Go:   err.Error()
来源：http://oeb.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://ksa.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://eak.hywenlv.cn

[H09] 带错误码的异常
来源：http://thp.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://agr.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtl.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://feo.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lku.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmm.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vdo.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://fje.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tiq.nanxinkj.top

[H10] 资源自动释放
来源：http://qdz.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zly.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fxv.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gix.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hos.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://noe.fzhhl.top

Go:   defer f.Close()
来源：http://zwn.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lsd.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afh.sufxvd.cn

================================================================================
来源：http://nfw.yuanzhike.top

I. 正则表达式
来源：http://omi.sufxvd.cn

================================================================================
来源：http://sjn.andypj.xyz

[I01] 判断是否匹配
来源：http://yxu.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qnj.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://ime.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ibj.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://gps.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xrn.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yhp.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://gig.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gxl.c1oappe.top

[I02] 提取所有匹配
来源：http://dlw.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://djl.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dzd.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wwx.uphjek.com

TS:   s.match(/\d+/g)
来源：http://euh.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vnb.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yzl.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://hmv.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yas.yangfankeji.com

[I03] 提取捕获分组
来源：http://ozh.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lwq.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ugx.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qaj.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gkd.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xdv.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xra.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfb.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zxi.ydzc1.top

[I04] 正则替换
来源：http://pgs.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://coy.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mje.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ryg.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fiv.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://vzt.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pkj.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nqk.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://opq.chenzaomai.com

[I05] 按正则拆分
来源：http://zpe.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ewu.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qki.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://xud.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://eay.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://fol.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lfj.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://usj.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ebz.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfm.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gpu.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cir.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ege.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jep.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nir.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://psi.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wwb.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mwq.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://pvv.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gjz.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://awx.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xen.cdnleiting.top

TS:   /error/gim
来源：http://gul.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ecc.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tra.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://bgj.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cis.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://yei.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lhz.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wqh.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://drk.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://exd.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tum.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgs.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mgz.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iqr.shanyushiyangkeji.top

================================================================================
来源：http://qqu.zhijiandao.cn

J. 日期与时间
来源：http://zrt.hammf.cn

================================================================================
来源：http://uex.xinyue.icu

[J01] 获取当前时间
来源：http://nkr.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vkh.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pkk.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://jze.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://pds.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qkl.gotoacloud.top

Go:   time.Now()
来源：http://wfm.epnwcf.com

Ruby: Time.now
来源：http://cxi.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixn.hnqzz.top

[J02] 格式化输出
来源：http://ppr.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dbc.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cvc.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tse.nanxinkj.top

TS:   d.toISOString()
来源：http://cix.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dex.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hjx.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxo.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://heh.epnwcf.com

[J03] 字符串解析为日期
来源：http://bmv.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hnq.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wcy.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://jos.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://ndt.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jxt.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jhx.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://fzd.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mpx.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://zxm.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fit.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vlx.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gli.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kcf.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cid.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ads.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ptt.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://adx.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://imz.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://mxd.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gpz.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpr.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hlk.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://nbg.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kvp.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://heh.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bja.xinyue.icu

[J06] 计算两时间之差
来源：http://zhi.yj20258.top


<!-- 参考信息 -->