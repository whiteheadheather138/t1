代发 wailian999

PHP:  public static function f() {}
来源：http://siv.redwolf501.top

JS:   static f() {}
来源：http://yge.kuanghao11.cn

TS:   static f(): void {}
来源：http://tmc.kuanghao11.cn

Java: static void f() {}
来源：http://ant.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bam.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://waa.hnxiangtu.top

C#:   public static void F() {}
来源：http://fbu.fehbvm.com

[G09] 接口 / 抽象类
来源：http://xlv.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://xou.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rgw.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://fnk.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://cmu.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://dmy.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://mvm.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dzp.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://jcn.fengsongda.top

[G10] 访问控制
来源：http://fed.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://rtx.yfazqb.com

PHP:  public / protected / private
来源：http://qev.sweek.top

JS:   #private 字段；其余公开
来源：http://fwz.gaohongyu789.top

TS:   public / protected / private
来源：http://crk.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://voz.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hul.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://pib.yueranfly.top

C#:   public / protected / private / internal
来源：http://viw.jinghuilouyu.cn

[G11] getter / setter
来源：http://fni.hammf.cn

Py:   @property 与 @x.setter
来源：http://mor.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://sms.havefunace.top

JS:   get name() { return this._name; }
来源：http://gxy.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://tcp.snrcjt.cn

Java: public String getName() { return name; }
来源：http://pms.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://soe.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://wih.uphjek.com

C#:   public string Name { get; set; }
来源：http://uoc.tarul.cn

[G12] 对象转字符串
来源：http://rqk.cashguo.top

Py:   def __str__(self): return self.name
来源：http://jph.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://zru.guannengcc.top

JS:   toString() { return this.name; }
来源：http://enk.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://kmy.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://tch.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://jqm.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://zpu.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://jio.cheryme.top

[G13] 判断对象类型
来源：http://vue.tian-w.cn

Py:   isinstance(u, User)
来源：http://pgu.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://zjn.sweek.top

JS:   u instanceof User
来源：http://kje.yuxming.cn

TS:   u instanceof User
来源：http://uze.tarul.cn

Java: u instanceof User
来源：http://pcr.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oos.guannengcc.top

Ruby: u.is_a?(User)
来源：http://olw.shzxlz.cn

C#:   u is User
来源：http://znl.shuidangran.top

[G14] 数据类 / record
来源：http://qoy.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hyw.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://unc.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://rea.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://mty.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://usf.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://nyi.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lbm.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://isj.shzxlz.cn

[G15] 枚举
来源：http://vnf.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://erj.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jgp.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gji.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogy.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://hwe.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rxe.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://jbd.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bhx.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://ptw.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qif.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://thr.epnwcf.com

JS:   Object.entries(obj)
来源：http://tqw.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://jfi.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qby.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bgj.meibo888.top

Ruby: obj.instance_variables
来源：http://lwb.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://vtl.sysykeji.top

================================================================================
来源：http://oob.gotoacloud.top

H. 异常与错误处理
来源：http://ffn.zhijiandao.cn

================================================================================
来源：http://vub.epnwcf.com

[H01] try / catch 基础
来源：http://jwu.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ddu.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fuh.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oaa.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ghd.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ryr.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mzh.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mxf.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ukw.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://jbq.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://tgu.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://djb.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wsp.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://sct.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://lvv.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ykx.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lgj.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ymj.ehwqpu.com

[H03] 主动抛出异常
来源：http://siu.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://rvh.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://axb.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://lnz.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://ipn.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hjb.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pbs.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mis.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://iiq.hywenlv.cn

[H04] 自定义异常类型
来源：http://gwa.316326.xyz

Py:   class MyError(Exception): pass
来源：http://pse.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zvz.ybcxt.top

JS:   class MyError extends Error {}
来源：http://ykm.yj202588.top

TS:   class MyError extends Error {}
来源：http://eag.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://bjd.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqu.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://vov.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://ldo.hysaishi.cn

[H05] 捕获特定类型
来源：http://blj.yvedp.cn

Py:   except ValueError as e:
来源：http://iwk.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynj.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://mrq.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://nfu.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://jvq.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aiq.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://bow.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cuu.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://taj.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://lrc.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://dnx.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://xja.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://gzy.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://snq.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tmt.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://dvh.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://szv.yj202588.top

[H07] 断言
来源：http://iba.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://qzm.haohaochexian.top

PHP:  assert($x > 0);
来源：http://ayz.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://dbu.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://wyj.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://pxq.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lrx.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://uju.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://spo.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://gov.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://exl.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qch.ctjpmb.com

JS:   e.message;  e.stack
来源：http://abg.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xri.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://soq.jinqigufen.top

Go:   err.Error()
来源：http://kqr.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://rtt.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://rca.shzxlz.cn

[H09] 带错误码的异常
来源：http://gpd.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lzu.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://imt.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qoq.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ghm.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nui.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oyr.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://bqj.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uvq.cashguo.top

[H10] 资源自动释放
来源：http://loh.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rno.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fat.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://owo.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://liu.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yzj.tanke756.top

Go:   defer f.Close()
来源：http://puf.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://btn.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vsj.sjlbkw.cn

================================================================================
来源：http://pyy.chenlongwang.top

I. 正则表达式
来源：http://nou.xinyue.icu

================================================================================
来源：http://jot.chenzaomai.com

[I01] 判断是否匹配
来源：http://sjo.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://afn.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://cxs.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://nxj.sweek.top

TS:   /\d+/.test(s)
来源：http://ggc.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yaf.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jdi.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://yrx.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://frm.nwbrower.top

[I02] 提取所有匹配
来源：http://wgp.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://hok.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://urm.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xvx.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://dmp.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xpw.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aqx.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://lvf.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gvj.gaohongyu789.top

[I03] 提取捕获分组
来源：http://qgx.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sod.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tdu.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://chl.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mjs.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uyw.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ngb.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mnw.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zjl.hammf.cn

[I04] 正则替换
来源：http://htt.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://gzd.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmv.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://mua.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://isp.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lqm.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yet.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cum.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cum.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://lnp.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://eeq.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hef.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://dgo.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://ciu.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://wyq.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fmw.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://fkj.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://inj.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zss.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nbr.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mpz.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://amm.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://igx.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://igg.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://amn.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lwi.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mhc.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://htt.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wgy.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vav.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ikb.chenzaomai.com

TS:   /error/gim
来源：http://swe.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ffz.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blv.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://fwn.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wnb.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://can.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ipb.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://doy.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckp.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekh.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tky.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wzr.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ttm.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://orz.52xcode.cn

================================================================================
来源：http://xfx.yfazqb.com

J. 日期与时间
来源：http://mvf.hammf.cn

================================================================================
来源：http://bgo.zhixingplan.top

[J01] 获取当前时间
来源：http://mbv.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xvt.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zfu.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://eov.xinyue.icu

TS:   new Date();  Date.now()
来源：http://qcx.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tmw.yueranfly.top

Go:   time.Now()
来源：http://uik.ppjwa.cn

Ruby: Time.now
来源：http://qvj.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ibq.aibaodan.cn

[J02] 格式化输出
来源：http://oov.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzg.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://plw.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dil.pengpengdd.cyou

TS:   d.toISOString()
来源：http://tkj.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvz.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kkc.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvy.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://scn.jianghu66.top

[J03] 字符串解析为日期
来源：http://ohq.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rpb.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uek.uphjek.com

JS:   new Date("2024-01-02")
来源：http://luh.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://gxx.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://dgy.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://slq.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://gyd.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://opj.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://dfw.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iiz.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uzd.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ccp.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://exu.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nna.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bxp.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wky.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eft.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://jqp.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://iiz.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eeg.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://prn.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jos.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://qvr.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ktm.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://vir.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yzr.tarul.cn

[J06] 计算两时间之差
来源：http://qyw.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://oib.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://fsu.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfl.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cqn.ehwqpu.com


<!-- 参考信息 -->