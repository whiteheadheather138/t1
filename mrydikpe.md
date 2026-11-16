代发 wailian999

PHP:  public static function f() {}
来源：http://lrh.havefunace.top

JS:   static f() {}
来源：http://lem.pycfn.com

TS:   static f(): void {}
来源：http://wjz.hywenlv.cn

Java: static void f() {}
来源：http://tko.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vew.jyoumei.cn

Ruby: def self.f; end
来源：http://ozy.birdmap.top

C#:   public static void F() {}
来源：http://nyl.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://qaz.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://nql.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hvi.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jxy.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://tjc.shuidangran.top

Java: interface Shape { double area(); }
来源：http://roa.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://tac.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rih.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://whf.epnwcf.com

[G10] 访问控制
来源：http://kpd.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://mtr.316326.xyz

PHP:  public / protected / private
来源：http://dml.ybcxt.top

JS:   #private 字段；其余公开
来源：http://hlh.smart0.xyz

TS:   public / protected / private
来源：http://rfp.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://qmq.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://thd.jqgufenzy.top

Ruby: public / protected / private
来源：http://bun.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://hnw.sysykeji.top

[G11] getter / setter
来源：http://wgf.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://tcx.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wlr.fengsongda.top

JS:   get name() { return this._name; }
来源：http://idm.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://nef.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://xll.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fln.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://htt.yongpay.top

C#:   public string Name { get; set; }
来源：http://hlb.hcnkem.com

[G12] 对象转字符串
来源：http://ayv.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://ozu.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://igy.xuanzx.com

JS:   toString() { return this.name; }
来源：http://jpn.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://yvw.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://mew.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tjh.tarul.cn

Ruby: def to_s; @name; end
来源：http://jlc.tarul.cn

C#:   public override string ToString() => Name;
来源：http://rkh.havefunace.top

[G13] 判断对象类型
来源：http://nql.aizwys.cn

Py:   isinstance(u, User)
来源：http://mwh.hysaishi.cn

PHP:  $u instanceof User
来源：http://fhr.ehwqpu.com

JS:   u instanceof User
来源：http://ryg.zhoulong.xyz

TS:   u instanceof User
来源：http://pet.zhixingplan.top

Java: u instanceof User
来源：http://bmm.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://inh.tarul.cn

Ruby: u.is_a?(User)
来源：http://wzf.yj20258888.top

C#:   u is User
来源：http://xqv.jianghu66.top

[G14] 数据类 / record
来源：http://icx.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gvp.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://csg.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xhj.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://lri.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://fas.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://uyy.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nct.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://jsg.yonumen.top

[G15] 枚举
来源：http://wae.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://edr.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sda.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zxg.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zno.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://bho.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmr.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://mcg.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://akp.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://fms.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pfw.tanke756.top

PHP:  get_object_vars($obj);
来源：http://ror.shzxlz.cn

JS:   Object.entries(obj)
来源：http://nur.daxiang520.top

TS:   Object.entries(obj)
来源：http://wsv.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://muy.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://erf.xylfe.cn

Ruby: obj.instance_variables
来源：http://ikp.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://ybs.sufxvd.cn

================================================================================
来源：http://nrt.jqgfzy.top

H. 异常与错误处理
来源：http://psr.wangshuangyany.cn

================================================================================
来源：http://qox.hfpthk.cn

[H01] try / catch 基础
来源：http://mws.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bxe.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wwa.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lot.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ipc.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://duj.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://usd.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uzq.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rrr.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://yun.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qgo.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffr.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uwl.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kqm.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://kik.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwr.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://rqx.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://luz.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://wlq.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://ehu.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hvq.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://lrq.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://ctd.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tjh.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kuj.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dyd.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://hjj.hnqzz.top

[H04] 自定义异常类型
来源：http://liy.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://buz.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://axv.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://kme.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://gvs.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://swd.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vhs.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://bxp.fktsv.cn

C#:   class MyException : Exception {}
来源：http://zgj.yj20258.top

[H05] 捕获特定类型
来源：http://pgp.wangdashe.top

Py:   except ValueError as e:
来源：http://jee.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rip.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://psb.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://bvj.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://hyv.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wll.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://zxz.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tob.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://wgq.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://sfn.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://ubq.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://tpy.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ggk.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xta.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xro.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://scp.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://dvo.vqdsnc.cn

[H07] 断言
来源：http://cuq.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://dpp.snrcjt.cn

PHP:  assert($x > 0);
来源：http://bjq.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://gby.jianghu66.top

TS:   console.assert(x > 0);
来源：http://cje.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://uqw.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ydc.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qlc.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://wkb.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://xny.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://hdr.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cnc.bjfxy.top

JS:   e.message;  e.stack
来源：http://iac.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://eok.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pvo.sjlbkw.cn

Go:   err.Error()
来源：http://fkq.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://gdl.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://exk.hnqzz.top

[H09] 带错误码的异常
来源：http://egt.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hwl.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oca.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://slv.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vdg.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vsp.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tbm.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dwn.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ntq.gogol.net.cn

[H10] 资源自动释放
来源：http://qee.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jtl.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eno.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://onh.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cam.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gaw.havefunace.top

Go:   defer f.Close()
来源：http://ldv.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iwe.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cet.svipenyu.cn

================================================================================
来源：http://apy.hysaishi.cn

I. 正则表达式
来源：http://qqs.chenjidiqi.icu

================================================================================
来源：http://pjh.fktsv.cn

[I01] 判断是否匹配
来源：http://nfm.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kag.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gvk.bbcook.cn

JS:   /\d+/.test(s)
来源：http://dfg.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://wmu.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tmi.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fge.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://gxh.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sbc.cashguo.top

[I02] 提取所有匹配
来源：http://guo.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://kzn.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://usw.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lpj.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://edw.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://azl.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://drf.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://hty.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://opi.ehwqpu.com

[I03] 提取捕获分组
来源：http://dkt.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqg.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://szz.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dyf.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ecr.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdn.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xho.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fzv.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hla.tian-w.cn

[I04] 正则替换
来源：http://yrc.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zej.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rqn.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://pdh.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://phe.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jtu.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://dsi.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iow.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tiv.feifeiyinyue.top

[I05] 按正则拆分
来源：http://dqd.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bnb.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cfn.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://agd.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://jqi.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://iiw.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ber.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://qcw.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tnt.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://acs.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uiy.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zka.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ino.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oue.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lng.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pro.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iub.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oxj.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://mcb.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://edz.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aon.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nzs.andypj.xyz

TS:   /error/gim
来源：http://erw.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zra.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hju.meibo888.top

Ruby: s.scan(/error/i)
来源：http://yfk.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yyc.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://bpe.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ucn.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ffi.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://elw.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwo.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gxs.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vwz.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yfs.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dcp.epnwcf.com

================================================================================
来源：http://yst.nanxinkj.top

J. 日期与时间
来源：http://ejl.xuetiantiany.cn

================================================================================
来源：http://wmo.sysykeji.top

[J01] 获取当前时间
来源：http://wgk.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nnz.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hgi.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://hjv.yj20258.top

TS:   new Date();  Date.now()
来源：http://omw.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rgh.mhx1999.top

Go:   time.Now()
来源：http://oqq.sweek.top

Ruby: Time.now
来源：http://dhp.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cms.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://bik.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://olj.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kdd.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pva.dianchejie.cn

TS:   d.toISOString()
来源：http://uca.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pvq.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hgi.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rds.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vhx.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://sxg.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pqh.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uvn.ivvv.top

JS:   new Date("2024-01-02")
来源：http://yls.yj202588.top

TS:   new Date("2024-01-02")
来源：http://mcs.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://mvi.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zfx.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://jdn.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eil.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://wdr.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://odh.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eho.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rzh.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zam.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wtn.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mqt.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://leq.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lyw.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://iua.316326.xyz

Py:   now + timedelta(days=7)
来源：http://kue.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://elq.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nga.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpc.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://llk.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aja.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ocw.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://zka.uphjek.com

[J06] 计算两时间之差
来源：http://wku.pycfn.com

Py:   (end - start).total_seconds()
来源：http://vsy.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://gcy.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://atd.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrs.hammf.cn


<!-- 参考信息 -->