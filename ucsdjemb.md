代发 wailian999

C#:   public / protected / private / internal
来源：http://khg.yonumen.top

[G11] getter / setter
来源：http://ozf.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://olg.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gdo.ydzc1.top

JS:   get name() { return this._name; }
来源：http://azu.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://qic.hnqzz.top

Java: public String getName() { return name; }
来源：http://cfg.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://siw.xuanzx.com

Ruby: attr_accessor :name
来源：http://cgw.bbcook.cn

C#:   public string Name { get; set; }
来源：http://bmw.xuanzx.com

[G12] 对象转字符串
来源：http://vkt.yj202588.top

Py:   def __str__(self): return self.name
来源：http://mtp.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fbh.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://fra.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://fwg.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://nbv.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://vlm.cashguo.top

Ruby: def to_s; @name; end
来源：http://lev.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://bco.dashuyun.cn

[G13] 判断对象类型
来源：http://ith.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://ncq.xziqi.cn

PHP:  $u instanceof User
来源：http://isv.haohaochexian.top

JS:   u instanceof User
来源：http://rrl.cqqwz.cn

TS:   u instanceof User
来源：http://acz.jinqigfzy.top

Java: u instanceof User
来源：http://frr.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zwn.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://khx.jiagoushi.top

C#:   u is User
来源：http://huk.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://aad.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fat.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://fjo.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://tbf.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://vtm.hnqzz.top

Java: record User(String name, int age) {}
来源：http://ozn.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://bht.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mgd.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://tpc.yuanzhike.top

[G15] 枚举
来源：http://nyo.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zkc.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bou.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ley.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wwe.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://mjm.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://msv.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://ljj.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vdn.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://mlv.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ixx.ivvv.top

PHP:  get_object_vars($obj);
来源：http://jlr.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://fiz.ctjpmb.com

TS:   Object.entries(obj)
来源：http://aap.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cfm.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ekb.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://rnt.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://sib.mhx1999.top

================================================================================
来源：http://zib.kuanghao11.cn

H. 异常与错误处理
来源：http://vgo.vehdjk.com

================================================================================
来源：http://fry.jlsjyb.cn

[H01] try / catch 基础
来源：http://kir.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ukm.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hee.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qlc.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mil.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dqb.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zml.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dgy.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ttp.yongpay.top

[H02] finally / ensure 收尾
来源：http://zco.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mqg.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tsj.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dmr.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ynw.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hjx.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mhv.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pmy.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ksl.snrcjt.cn

[H03] 主动抛出异常
来源：http://syv.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://aha.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zoe.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://may.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://oks.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eaz.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://elv.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rry.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fjh.9152youxi.cn

[H04] 自定义异常类型
来源：http://nyh.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://dlb.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://isa.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://srx.zycfv.cn

TS:   class MyError extends Error {}
来源：http://nip.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://zsk.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lsi.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://chg.shuidangran.top

C#:   class MyException : Exception {}
来源：http://mnz.tarul.cn

[H05] 捕获特定类型
来源：http://xsc.shuidangran.top

Py:   except ValueError as e:
来源：http://gxz.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://izb.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://ltu.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://fmz.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://yaa.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kcr.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://uhv.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://osq.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://vnd.xinyue.icu

Py:   value = d.get("k") or default
来源：http://kbr.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://tvx.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://voj.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pzw.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://arj.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://api.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://yse.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://ssh.dashuyun.cn

[H07] 断言
来源：http://unr.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://wwy.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://xne.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://djj.fktsv.cn

TS:   console.assert(x > 0);
来源：http://oej.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://mgs.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kbc.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uul.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://xdu.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://jvz.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://isj.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kpn.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://sks.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lka.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kzr.fehbvm.com

Go:   err.Error()
来源：http://baz.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://ujh.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://rmh.9152youxi.cn

[H09] 带错误码的异常
来源：http://mtc.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wqn.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gmc.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zne.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tvt.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kee.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nnv.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://osd.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hir.chenlongwang.top

[H10] 资源自动释放
来源：http://krh.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lec.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hne.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kkm.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rus.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyd.cqqwz.cn

Go:   defer f.Close()
来源：http://uzi.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ucj.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kpv.fktsv.cn

================================================================================
来源：http://yfn.xingfuxueyuan.xyz

I. 正则表达式
来源：http://clh.uphjek.com

================================================================================
来源：http://don.vqdsnc.cn

[I01] 判断是否匹配
来源：http://ntf.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pca.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://kyh.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://lea.nwbrower.top

TS:   /\d+/.test(s)
来源：http://omv.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zyo.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ihy.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://qew.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vof.316326.xyz

[I02] 提取所有匹配
来源：http://vos.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://lpe.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lng.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zvm.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://dda.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vyx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qzu.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://knu.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cid.jianghu66.top

[I03] 提取捕获分组
来源：http://qnv.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://orn.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gud.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cxf.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://olt.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://obr.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qzk.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qaa.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vxe.yj20258.top

[I04] 正则替换
来源：http://uaa.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://guo.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kbs.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://pnq.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rrr.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://ugn.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hoa.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nif.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nkr.hesvh.cn

[I05] 按正则拆分
来源：http://rvl.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://blz.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://och.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://rcf.zdqjudy.top

TS:   s.split(/\s*,\s*/)
来源：http://svx.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://uaq.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://otd.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://mnh.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gwz.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wfo.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uat.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ipl.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ocy.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ool.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bcc.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jks.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kxj.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kkr.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://gya.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hek.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://coe.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cmq.hywenlv.cn

TS:   /error/gim
来源：http://lro.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lsc.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qhx.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://vbs.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://toh.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://tdx.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vjq.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iqh.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eht.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eud.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://oyk.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kig.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dun.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zsy.feifeiyinyue.top

================================================================================
来源：http://rda.tanke756.top

J. 日期与时间
来源：http://sal.zhoulong.xyz

================================================================================
来源：http://uzl.ctjpmb.com

[J01] 获取当前时间
来源：http://boe.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ckh.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yis.316326.xyz

JS:   new Date();  Date.now()
来源：http://dtt.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://ubb.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kie.wangdashe.top

Go:   time.Now()
来源：http://iis.zhoulong.xyz

Ruby: Time.now
来源：http://gvt.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vqy.zhoulong.xyz

[J02] 格式化输出
来源：http://bfl.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usb.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ivv.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vlw.yonumen.top

TS:   d.toISOString()
来源：http://xqk.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xvo.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vmi.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfg.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://clp.guowangkeji.top

[J03] 字符串解析为日期
来源：http://dkd.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pre.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cov.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://euu.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://ufh.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://qta.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fyq.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://qpr.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hym.guannengcc.top

[J04] 时间戳与日期互转
来源：http://bkz.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xdq.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tkc.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pwc.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lsw.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fla.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xpi.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kks.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ncv.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://gpw.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://lom.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cbk.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qed.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ucm.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://vnv.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emq.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://uzq.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://wer.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://jdu.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://vpc.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://hmq.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wmt.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cce.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://keq.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://ufk.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://nxw.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://iwg.tian-w.cn

[J07] 比较两个日期
来源：http://zku.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://adf.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ars.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://hzt.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://urd.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uch.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jds.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jbj.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://ign.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://obk.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ymj.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cha.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xyx.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wdl.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uai.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gap.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://azn.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xte.fktsv.cn

[J09] 时区处理
来源：http://okh.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qzf.sweek.top


<!-- 参考信息 -->