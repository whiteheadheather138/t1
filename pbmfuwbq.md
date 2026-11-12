代发 wailian999

JS:   super.greet();
来源：http://amj.c1oappe.top

TS:   super.greet();
来源：http://eqb.chenzaomai.com

Java: super.greet();
来源：http://rle.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uwc.yfazqb.com

Ruby: super
来源：http://yya.ydjk.org.cn

C#:   base.Greet();
来源：http://hap.smart0.xyz

[G08] 静态方法与属性
来源：http://yqw.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gxa.cdnleiting.top

PHP:  public static function f() {}
来源：http://yks.zhoulong.xyz

JS:   static f() {}
来源：http://wlv.zdbjq.cn

TS:   static f(): void {}
来源：http://ecp.svipenyu.cn

Java: static void f() {}
来源：http://zrk.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jpm.ppjwa.cn

Ruby: def self.f; end
来源：http://kkx.xinyue.icu

C#:   public static void F() {}
来源：http://gua.cucudq.cn

[G09] 接口 / 抽象类
来源：http://pjv.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://rqn.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://tup.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uxk.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://cnt.mhx1999.top

Java: interface Shape { double area(); }
来源：http://tqc.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://aze.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nec.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://jva.xziqi.cn

[G10] 访问控制
来源：http://wfl.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://ywu.sweek.top

PHP:  public / protected / private
来源：http://gtk.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://eso.cheryme.top

TS:   public / protected / private
来源：http://zsw.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://xxq.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://htr.wangdashe.top

Ruby: public / protected / private
来源：http://oro.fehbvm.com

C#:   public / protected / private / internal
来源：http://hej.ppjwa.cn

[G11] getter / setter
来源：http://tja.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://wsp.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://woi.hcnkem.com

JS:   get name() { return this._name; }
来源：http://lew.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://gjt.cdnleiting.top

Java: public String getName() { return name; }
来源：http://gye.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://twc.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://nux.ydzc1.top

C#:   public string Name { get; set; }
来源：http://axs.zdqjudy.top

[G12] 对象转字符串
来源：http://poo.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://boy.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rpo.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://zef.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://afb.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://zul.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yzs.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://sku.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://kmk.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://zmc.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://aba.ehwqpu.com

PHP:  $u instanceof User
来源：http://tmz.aibaodan.cn

JS:   u instanceof User
来源：http://akg.haohaochexian.top

TS:   u instanceof User
来源：http://nez.xziqi.cn

Java: u instanceof User
来源：http://lnk.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zab.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://cgk.yangfankeji.com

C#:   u is User
来源：http://kpx.havefunace.top

[G14] 数据类 / record
来源：http://umo.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vps.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://fah.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://dni.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://odu.fengsongda.top

Java: record User(String name, int age) {}
来源：http://red.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://ryn.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sfd.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://kpy.cqqwz.cn

[G15] 枚举
来源：http://ssp.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://teq.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lbf.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mxw.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://njy.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://fyw.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ywz.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://epn.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vwb.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://gkq.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jzf.yongpay.top

PHP:  get_object_vars($obj);
来源：http://onp.zhixingplan.top

JS:   Object.entries(obj)
来源：http://ujr.ppjwa.cn

TS:   Object.entries(obj)
来源：http://fay.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://glp.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://whb.bbcook.cn

Ruby: obj.instance_variables
来源：http://doq.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://tme.shanyushiyangkeji.top

================================================================================
来源：http://oba.hammf.cn

H. 异常与错误处理
来源：http://gzn.vehdjk.com

================================================================================
来源：http://uyw.jlsjyb.cn

[H01] try / catch 基础
来源：http://ysg.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxx.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nsf.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kmh.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lba.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kor.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dcl.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lfz.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jnw.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://ewa.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://vdc.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dzq.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bwj.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zyc.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://awc.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xgz.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cli.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://seo.jinqigufen.top

[H03] 主动抛出异常
来源：http://ukv.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://awj.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rrk.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://zbc.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://szr.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wfo.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://upp.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xil.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://plc.ybcxt.top

[H04] 自定义异常类型
来源：http://utg.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://vrd.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://lqg.uphjek.com

JS:   class MyError extends Error {}
来源：http://abc.gzhubu.top

TS:   class MyError extends Error {}
来源：http://gmn.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://rgz.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xhd.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://ixw.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://rku.xuanzx.com

[H05] 捕获特定类型
来源：http://cwi.bjfxy.top

Py:   except ValueError as e:
来源：http://taq.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oex.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://gun.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://ewt.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://xsq.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pdl.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://nju.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rfv.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://gbb.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://wpb.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://crf.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://fen.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cdp.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jjp.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oxx.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://isy.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://xyz.ydzc1.top

[H07] 断言
来源：http://btq.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://qpd.dianchejie.cn

PHP:  assert($x > 0);
来源：http://nyx.yfazqb.com

JS:   console.assert(x > 0);
来源：http://lfk.hammf.cn

TS:   console.assert(x > 0);
来源：http://fdq.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://sip.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lap.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://qao.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://ecn.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://yfx.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://pch.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pyl.jqgfzy.top

JS:   e.message;  e.stack
来源：http://vym.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kqb.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zsz.ywan-chungtsiang.top

Go:   err.Error()
来源：http://uuf.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://agj.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://qtf.sufxvd.cn

[H09] 带错误码的异常
来源：http://jdp.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bjd.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hgs.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhq.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqn.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffj.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iie.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://qaz.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lfv.ybcxt.top

[H10] 资源自动释放
来源：http://tnr.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fxd.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://axc.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rvi.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://umr.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oxl.cqqwz.cn

Go:   defer f.Close()
来源：http://zqm.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fmi.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dql.zhaomingkeji.xyz

================================================================================
来源：http://nzi.yj202588.top

I. 正则表达式
来源：http://oiw.cashguo.top

================================================================================
来源：http://nkl.ydzc1.top

[I01] 判断是否匹配
来源：http://lpx.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fkk.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xjl.jianghu66.top

JS:   /\d+/.test(s)
来源：http://gkj.meibo888.top

TS:   /\d+/.test(s)
来源：http://xmj.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwp.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://whj.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://dxn.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vpx.9152youxi.cn

[I02] 提取所有匹配
来源：http://lvx.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://fed.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://waj.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ldm.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://lxg.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bcf.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://loa.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://ics.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vca.jianghu66.top

[I03] 提取捕获分组
来源：http://zut.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lur.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cod.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyf.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kmn.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qxb.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hzy.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gwv.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nsp.cqqwz.cn

[I04] 正则替换
来源：http://ddv.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mny.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uck.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hlo.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hpl.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://crz.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jry.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nhz.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aiw.bjfxy.top

[I05] 按正则拆分
来源：http://ifb.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fzj.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bdv.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://utz.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://mgl.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://wtc.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hjj.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://dpx.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bpv.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://law.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lbr.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mtu.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhn.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ptt.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fcr.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ymq.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lke.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsz.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://eyi.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ggm.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rjz.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wka.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://mfq.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nne.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rps.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://oie.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://poh.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://ysj.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://quj.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://grh.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rvo.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ksp.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xrh.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kcp.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mau.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vkt.cdnleiting.top

================================================================================
来源：http://jmt.nwbrower.top

J. 日期与时间
来源：http://cat.chenzaomai.com

================================================================================
来源：http://gfx.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://udr.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oit.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://leb.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://eez.ybcxt.top

TS:   new Date();  Date.now()
来源：http://ain.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kvr.cdnleiting.top

Go:   time.Now()
来源：http://luv.nanxuanxn.top

Ruby: Time.now
来源：http://aus.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fyc.havefunace.top

[J02] 格式化输出
来源：http://eqe.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjf.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ddm.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zqn.chenjidiqi.icu

TS:   d.toISOString()
来源：http://ikr.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lzr.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xpk.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyu.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://llz.pycfn.com

[J03] 字符串解析为日期
来源：http://lhi.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gkd.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ghl.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://lcn.cheryme.top

TS:   new Date("2024-01-02")
来源：http://shc.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qjx.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jyl.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://mdf.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mzw.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://bzm.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bam.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mzf.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qei.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jfc.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://arm.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://akm.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dua.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://roq.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://acs.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://ffs.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uco.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qjt.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltz.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://ijx.svipenyu.cn


<!-- 参考信息 -->