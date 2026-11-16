代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://mov.snrcjt.cn

Ruby: def self.f; end
来源：http://bou.yj20258888.top

C#:   public static void F() {}
来源：http://nud.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://ria.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://zgc.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://cqv.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://agq.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://xzj.yueranfly.top

Java: interface Shape { double area(); }
来源：http://sde.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://aiy.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xgx.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://ukp.ybcxt.top

[G10] 访问控制
来源：http://iem.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://nuk.xinyue.icu

PHP:  public / protected / private
来源：http://nzv.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://exe.xylfe.cn

TS:   public / protected / private
来源：http://yyt.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://nem.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eme.jinqigufen.top

Ruby: public / protected / private
来源：http://lfd.smart0.xyz

C#:   public / protected / private / internal
来源：http://ygn.birdmap.top

[G11] getter / setter
来源：http://lxa.meibo888.top

Py:   @property 与 @x.setter
来源：http://ikd.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fqn.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://xes.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://khz.316326.xyz

Java: public String getName() { return name; }
来源：http://hme.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://egs.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://ooh.hnqzz.top

C#:   public string Name { get; set; }
来源：http://nbn.zdbjq.cn

[G12] 对象转字符串
来源：http://jrm.tarul.cn

Py:   def __str__(self): return self.name
来源：http://pog.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcw.fktsv.cn

JS:   toString() { return this.name; }
来源：http://quo.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://dho.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://qvg.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://oif.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://fdb.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://oei.sufxvd.cn

[G13] 判断对象类型
来源：http://qwj.hfpthk.cn

Py:   isinstance(u, User)
来源：http://xqt.fzhhl.top

PHP:  $u instanceof User
来源：http://uro.ybcxt.top

JS:   u instanceof User
来源：http://ebu.zhiwuduotai.top

TS:   u instanceof User
来源：http://ozc.sjlbkw.cn

Java: u instanceof User
来源：http://gwo.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eum.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://omz.jqgufenzy.top

C#:   u is User
来源：http://dkx.yj202588.top

[G14] 数据类 / record
来源：http://spj.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xwe.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://sbu.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aaj.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://fwk.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://rmf.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://ltw.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mzw.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://pkj.wangshuangyany.cn

[G15] 枚举
来源：http://qet.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mis.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pgc.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lfz.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nkn.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://pga.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xzw.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://ssq.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://olj.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://ysp.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vpv.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://wzu.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://zpg.sufxvd.cn

TS:   Object.entries(obj)
来源：http://meo.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mls.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pzb.aibaodan.cn

Ruby: obj.instance_variables
来源：http://jna.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://aao.zycfv.cn

================================================================================
来源：http://ywx.hfpthk.cn

H. 异常与错误处理
来源：http://rqn.daria6918.cn

================================================================================
来源：http://bcg.guowangkeji.top

[H01] try / catch 基础
来源：http://aav.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://trd.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wpq.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uwn.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lkv.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xim.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kgr.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bll.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zme.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://jbh.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qvl.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lyz.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gac.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lqk.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://pft.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eun.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://utt.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lys.jianghu66.top

[H03] 主动抛出异常
来源：http://owb.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://vif.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kee.jqgfzy.top

JS:   throw new Error("错误信息");
来源：http://msc.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://qyt.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://cvz.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fcy.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lru.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tfv.vehdjk.com

[H04] 自定义异常类型
来源：http://xjm.52xcode.cn

Py:   class MyError(Exception): pass
来源：http://fye.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uxj.vehdjk.com

JS:   class MyError extends Error {}
来源：http://mwq.c1oappe.top

TS:   class MyError extends Error {}
来源：http://zqh.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://nvt.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://chf.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://zjy.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://epx.tian-w.cn

[H05] 捕获特定类型
来源：http://wib.xziqi.cn

Py:   except ValueError as e:
来源：http://qfz.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ieb.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://gvj.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://cwg.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://npf.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvn.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://xaj.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eyo.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://zfm.bbcook.cn

Py:   value = d.get("k") or default
来源：http://jkz.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://axj.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://brl.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://llo.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iwl.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cxd.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://xyj.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://uby.nanxuanxn.top

[H07] 断言
来源：http://xsx.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://ydk.gotoacloud.top

PHP:  assert($x > 0);
来源：http://oee.pycfn.com

JS:   console.assert(x > 0);
来源：http://wvv.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://vnq.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://vtz.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wwo.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://drf.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://dsr.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://are.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ega.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iag.guannengcc.top

JS:   e.message;  e.stack
来源：http://jud.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://koe.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://htg.zhaomingkeji.xyz

Go:   err.Error()
来源：http://bvu.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://vyg.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ibg.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://rqo.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lyc.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://clm.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lmz.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://stn.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wmi.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nkg.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wjc.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://toh.sjlbkw.cn

[H10] 资源自动释放
来源：http://ruh.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oeb.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rfq.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jpx.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tar.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ceq.zycfv.cn

Go:   defer f.Close()
来源：http://yxw.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jjp.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hrz.ctjpmb.com

================================================================================
来源：http://ujb.gzhubu.top

I. 正则表达式
来源：http://bjm.jiagoushi.top

================================================================================
来源：http://txy.daxiang520.top

[I01] 判断是否匹配
来源：http://jis.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://byi.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://sgw.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://wwf.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://byp.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xpo.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wzj.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://ysc.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cvx.zhengqikj.top

[I02] 提取所有匹配
来源：http://ojv.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://nfc.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ghc.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pid.tarul.cn

TS:   s.match(/\d+/g)
来源：http://bxs.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dvl.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ftq.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://qrt.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bsn.sjlbkw.cn

[I03] 提取捕获分组
来源：http://rfi.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://srr.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rrw.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kpn.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehc.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pry.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ibh.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://seg.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://utn.tarul.cn

[I04] 正则替换
来源：http://oxl.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hyx.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lfe.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://yyh.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://uiw.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://zee.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bsr.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nlu.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bii.yuanzhike.top

[I05] 按正则拆分
来源：http://vyf.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mvi.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pck.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://bzf.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://buw.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://mpz.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://egt.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://itu.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://klo.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tsf.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ewm.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sej.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywz.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zdg.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://awo.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dvx.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://roz.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gvb.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://ppe.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ogj.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mtl.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uay.nanxuanxn.top

TS:   /error/gim
来源：http://ufo.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cpm.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ipk.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://xuo.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://shd.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://huv.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pla.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gev.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gon.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uyr.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fxq.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xgl.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yld.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pow.xuetiantiany.cn

================================================================================
来源：http://lrs.fehbvm.com

J. 日期与时间
来源：http://ymh.aizwys.cn

================================================================================
来源：http://xqn.jyoumei.cn

[J01] 获取当前时间
来源：http://ugm.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rhq.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lqw.birdmap.top

JS:   new Date();  Date.now()
来源：http://bhl.daxiang520.top

TS:   new Date();  Date.now()
来源：http://lhu.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uiu.ppjwa.cn

Go:   time.Now()
来源：http://avx.hnxiangtu.top

Ruby: Time.now
来源：http://iwp.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nau.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://uqo.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jnt.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kko.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xcf.yueranfly.top

TS:   d.toISOString()
来源：http://zcn.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rnj.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://llg.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwy.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kwl.guannengcc.top

[J03] 字符串解析为日期
来源：http://fhf.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bai.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://crn.meibo888.top

JS:   new Date("2024-01-02")
来源：http://ajo.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://utr.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iyx.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cgn.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://aae.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckp.epnwcf.com

[J04] 时间戳与日期互转
来源：http://kdf.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ods.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dbv.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jxz.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gyd.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iuq.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wif.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dvc.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jko.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://fhx.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://vrr.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://yyx.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fbz.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cot.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://tjd.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qat.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://gbe.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zgp.uphjek.com

[J06] 计算两时间之差
来源：http://zrh.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://bfu.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://vmu.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfo.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://whr.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://yfm.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://kjh.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://lrp.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://dvq.tianlin.xyz


<!-- 参考信息 -->