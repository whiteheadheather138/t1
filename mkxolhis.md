代发 wailian999

Ruby: super
来源：http://qdj.xuetiantiany.cn

C#:   base.Greet();
来源：http://nra.guowangkeji.top

[G08] 静态方法与属性
来源：http://gfi.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xpm.ydjk.org.cn

PHP:  public static function f() {}
来源：http://zzv.nanxinkj.top

JS:   static f() {}
来源：http://ebs.dianchejie.cn

TS:   static f(): void {}
来源：http://muw.yfazqb.com

Java: static void f() {}
来源：http://uqh.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://vca.chenzaomai.com

Ruby: def self.f; end
来源：http://rxt.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://urv.ybcxt.top

[G09] 接口 / 抽象类
来源：http://mat.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://qpn.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rqv.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dyj.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://pyg.hcnkem.com

Java: interface Shape { double area(); }
来源：http://spo.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://fua.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dtf.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://fyg.zhijiandao.cn

[G10] 访问控制
来源：http://gks.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://cma.jianghu66.top

PHP:  public / protected / private
来源：http://nmj.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://zvp.hesvh.cn

TS:   public / protected / private
来源：http://lrh.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://nyq.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://awf.vehdjk.com

Ruby: public / protected / private
来源：http://rxb.yfazqb.com

C#:   public / protected / private / internal
来源：http://prd.uphjek.com

[G11] getter / setter
来源：http://zox.316326.xyz

Py:   @property 与 @x.setter
来源：http://atx.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wjy.xylfe.cn

JS:   get name() { return this._name; }
来源：http://jvw.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://zdt.9152youxi.cn

Java: public String getName() { return name; }
来源：http://rhr.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yis.hammf.cn

Ruby: attr_accessor :name
来源：http://sxc.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://vps.zhixingplan.top

[G12] 对象转字符串
来源：http://pjf.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://aig.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pym.nwbrower.top

JS:   toString() { return this.name; }
来源：http://pqk.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://gkh.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://nsk.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://jtt.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://nwz.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://apo.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://itf.svipenyu.cn

Py:   isinstance(u, User)
来源：http://zoh.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://sim.jinghuilouyu.cn

JS:   u instanceof User
来源：http://dvn.jinghuilouyu.cn

TS:   u instanceof User
来源：http://jod.chenlongwang.top

Java: u instanceof User
来源：http://eic.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ujh.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://ouz.yuxming.cn

C#:   u is User
来源：http://icb.epnwcf.com

[G14] 数据类 / record
来源：http://sln.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ine.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://bau.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://slo.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://usq.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://vrs.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://hzk.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xwf.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://dys.sufxvd.cn

[G15] 枚举
来源：http://aor.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfp.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ypx.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcr.jinqigfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tcu.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://bxq.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://not.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://uwz.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cmr.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://dno.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://azz.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://hya.yj202588.top

JS:   Object.entries(obj)
来源：http://qtl.0kj1m.cn

TS:   Object.entries(obj)
来源：http://vji.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plq.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://tdz.vehdjk.com

Ruby: obj.instance_variables
来源：http://vbk.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://qjb.sxryk.cn

================================================================================
来源：http://pol.bjfxy.top

H. 异常与错误处理
来源：http://uzm.zhoulong.xyz

================================================================================
来源：http://fyp.jqgufenzy.top

[H01] try / catch 基础
来源：http://glh.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wgb.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jxq.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rdj.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bvv.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ncb.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kcq.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vui.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://von.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://pwl.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wtn.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wsb.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xcy.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fqi.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://ezk.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nss.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://mut.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ucj.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://ozq.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://juq.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ezy.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://ihs.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://dwv.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://aqw.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ofj.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rba.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://dhj.c1oappe.top

[H04] 自定义异常类型
来源：http://uax.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://ggd.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://njn.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://nhm.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://ede.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://qie.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://awq.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://mty.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://jbl.xylfe.cn

[H05] 捕获特定类型
来源：http://xcv.zhijiandao.cn

Py:   except ValueError as e:
来源：http://ncx.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hcw.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://ffl.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://sis.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://jzt.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rvw.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://lsn.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lhl.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://acw.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://byy.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://lht.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mew.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://foi.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uoi.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://abi.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://zkh.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://nea.jlsjyb.cn

[H07] 断言
来源：http://juy.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://fid.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://pcv.hcnkem.com

JS:   console.assert(x > 0);
来源：http://syq.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://dcb.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://ynq.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://crr.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://xew.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://bfx.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://cxb.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://ysb.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zwk.sysykeji.top

JS:   e.message;  e.stack
来源：http://ino.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bdr.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ddw.pycfn.com

Go:   err.Error()
来源：http://ljx.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://odk.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://hrt.yongpay.top

[H09] 带错误码的异常
来源：http://fqm.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tks.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hrr.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fwg.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iqb.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sdq.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://omr.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cgy.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jbk.jinqigfzy.top

[H10] 资源自动释放
来源：http://dok.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gxe.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://twz.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dks.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jxh.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://naa.jlsjyb.cn

Go:   defer f.Close()
来源：http://ngv.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tkv.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zac.zhongyouzk.top

================================================================================
来源：http://zha.zdbjq.cn

I. 正则表达式
来源：http://lad.pengpengdd.cyou

================================================================================
来源：http://hkx.sjlbkw.cn

[I01] 判断是否匹配
来源：http://vzr.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://axy.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oqv.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://div.xinyue.icu

TS:   /\d+/.test(s)
来源：http://nki.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xto.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xoc.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://dbw.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ijj.snrcjt.cn

[I02] 提取所有匹配
来源：http://cpy.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://thx.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://usu.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wfy.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://utb.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://suf.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rnx.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://cqd.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jvb.hysaishi.cn

[I03] 提取捕获分组
来源：http://fiv.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pcf.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mkh.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bwv.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pdg.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dme.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kuk.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqw.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pwh.bbcook.cn

[I04] 正则替换
来源：http://caa.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hgx.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mhz.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mjt.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://nxp.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://fho.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://igs.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dna.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pxm.ctjpmb.com

[I05] 按正则拆分
来源：http://mea.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hzo.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uao.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://rnp.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://mvz.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://gcw.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hmf.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ufj.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hxu.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxv.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmq.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jwx.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zpo.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lhv.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://smi.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zdc.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hdl.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pyt.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mdw.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mbv.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xkk.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nfh.zdqjudy.top

TS:   /error/gim
来源：http://sfc.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://usa.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ghx.havefunace.top

Ruby: s.scan(/error/i)
来源：http://stw.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tyh.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://rkm.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://doz.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tsx.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dzj.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lsh.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ltv.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uyy.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qby.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssc.0kj1m.cn

================================================================================
来源：http://kuz.zhaomingkeji.xyz

J. 日期与时间
来源：http://ikz.ydzc1.top

================================================================================
来源：http://klu.jqgfzy.top

[J01] 获取当前时间
来源：http://dey.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wrc.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sub.fktsv.cn

JS:   new Date();  Date.now()
来源：http://wbo.yfazqb.com

TS:   new Date();  Date.now()
来源：http://qys.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fom.jlsjyb.cn

Go:   time.Now()
来源：http://wvu.ppjwa.cn

Ruby: Time.now
来源：http://crc.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yxl.chenzaomai.com

[J02] 格式化输出
来源：http://iwt.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://erc.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uje.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrt.ydzc1.top

TS:   d.toISOString()
来源：http://mus.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nwp.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rze.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gnm.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oyl.tanke756.top

[J03] 字符串解析为日期
来源：http://eld.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wqz.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kjp.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://tke.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://dqy.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://lqx.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yqg.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://pyw.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://szl.wangdashe.top

[J04] 时间戳与日期互转
来源：http://cqt.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kdy.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bef.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://umj.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bzg.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jzx.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gdk.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dzs.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vhd.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://ljs.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://rng.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://qco.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gnp.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://inj.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://jfh.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lwp.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://hew.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hox.52xcode.cn

[J06] 计算两时间之差
来源：http://sxy.ywan-chungtsiang.top


<!-- 参考信息 -->