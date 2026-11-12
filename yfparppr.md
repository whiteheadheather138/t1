代发 wailian999

Ruby: attr_accessor :name
来源：http://sjb.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://xsy.hesvh.cn

[G12] 对象转字符串
来源：http://qye.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://mqa.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mex.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://saj.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://tpw.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://mty.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://utn.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://cux.ivvv.top

C#:   public override string ToString() => Name;
来源：http://pim.dashuyun.cn

[G13] 判断对象类型
来源：http://uex.cqqwz.cn

Py:   isinstance(u, User)
来源：http://nub.nanxuanxn.top

PHP:  $u instanceof User
来源：http://ifu.cashguo.top

JS:   u instanceof User
来源：http://kkw.bbcook.cn

TS:   u instanceof User
来源：http://rdt.guannengcc.top

Java: u instanceof User
来源：http://khe.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fmz.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://fuw.yueranfly.top

C#:   u is User
来源：http://zjw.nanxinkj.top

[G14] 数据类 / record
来源：http://mmq.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://brk.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://ovc.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://wma.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://isa.guannengcc.top

Java: record User(String name, int age) {}
来源：http://zqt.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://cci.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xbs.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://yfv.jqgufenzy.top

[G15] 枚举
来源：http://htr.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bwa.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://quj.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tos.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dwd.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://feo.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://unv.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://zwd.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://two.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://rlt.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://brx.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://sif.0kj1m.cn

JS:   Object.entries(obj)
来源：http://aej.hcnkem.com

TS:   Object.entries(obj)
来源：http://ubz.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rff.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://emj.zycfv.cn

Ruby: obj.instance_variables
来源：http://yqx.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://rce.jlsjyb.cn

================================================================================
来源：http://obf.jqgfzy.top

H. 异常与错误处理
来源：http://noy.chenzaomai.com

================================================================================
来源：http://txo.hesvh.cn

[H01] try / catch 基础
来源：http://jgm.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://trt.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://npf.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gpf.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://azf.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxi.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ehb.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dve.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gce.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://sdr.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://osq.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://irh.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://uxx.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://iht.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://rch.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dpo.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dvx.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wkn.havefunace.top

[H03] 主动抛出异常
来源：http://tqk.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://zkj.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bnt.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://rgk.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://mjx.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cus.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tkl.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://shl.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ixl.xylfe.cn

[H04] 自定义异常类型
来源：http://zad.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://ynj.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://pka.yfazqb.com

JS:   class MyError extends Error {}
来源：http://dda.iojbl.cn

TS:   class MyError extends Error {}
来源：http://gnz.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://sjk.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bgj.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://etu.xinyue.icu

C#:   class MyException : Exception {}
来源：http://lij.snrcjt.cn

[H05] 捕获特定类型
来源：http://lcj.dashuyun.cn

Py:   except ValueError as e:
来源：http://jsa.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fyv.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://uqh.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://szc.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://rxs.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qda.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://tpi.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://luj.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://zvp.fzhhl.top

Py:   value = d.get("k") or default
来源：http://atp.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://bif.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://ack.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://wyp.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rhp.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://miq.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://fpc.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://ynl.fanxiaobao.xyz

[H07] 断言
来源：http://byk.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://bxs.birdmap.top

PHP:  assert($x > 0);
来源：http://soy.tanke756.top

JS:   console.assert(x > 0);
来源：http://kfi.fehbvm.com

TS:   console.assert(x > 0);
来源：http://yfv.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://kha.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ljc.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wbt.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://jov.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://doi.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://xbd.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ema.tianlin.xyz

JS:   e.message;  e.stack
来源：http://jjc.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://rel.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mvo.yfazqb.com

Go:   err.Error()
来源：http://liy.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://fdk.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://qpr.nanxuanxn.top

[H09] 带错误码的异常
来源：http://nfd.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lvk.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zki.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vdx.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eps.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://isn.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ixf.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://mpk.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dwz.zhengqikj.top

[H10] 资源自动释放
来源：http://sct.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyf.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://edm.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jce.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zsj.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fpp.hfpthk.cn

Go:   defer f.Close()
来源：http://zzu.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fql.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://haz.vqdsnc.cn

================================================================================
来源：http://qrd.dianchejie.cn

I. 正则表达式
来源：http://ibk.sufxvd.cn

================================================================================
来源：http://krh.haohaochexian.top

[I01] 判断是否匹配
来源：http://jjq.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jor.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://kux.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://shb.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://btj.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wfb.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nmj.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://euq.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ouy.yongpay.top

[I02] 提取所有匹配
来源：http://ziu.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://mub.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pzk.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rfc.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://dqu.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xky.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://brg.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://kgq.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mgc.guannengcc.top

[I03] 提取捕获分组
来源：http://qny.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xmt.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://opf.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qov.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kuf.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://asn.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ogx.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kcg.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xfi.chenjidiqi.icu

[I04] 正则替换
来源：http://sur.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://kpb.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://apr.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hrc.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://kie.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ttj.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gye.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uux.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sjq.ehwqpu.com

[I05] 按正则拆分
来源：http://xst.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mms.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eth.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://cxs.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://eqd.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://mik.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pus.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://nou.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mfu.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fxn.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qpw.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zys.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kiq.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://htv.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pmi.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehe.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://emy.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lab.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://ttk.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bja.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wll.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ujs.cucudq.cn

TS:   /error/gim
来源：http://hzk.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ivp.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://puo.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://lan.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qvj.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://gyb.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vcv.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qsd.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ltn.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://puw.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mef.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rbg.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xwu.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://egr.tarul.cn

================================================================================
来源：http://bdx.jqgufenzy.top

J. 日期与时间
来源：http://fqa.yongpay.top

================================================================================
来源：http://wbn.yvedp.cn

[J01] 获取当前时间
来源：http://cbs.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fxq.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gzq.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://wtp.hesvh.cn

TS:   new Date();  Date.now()
来源：http://rhc.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pen.ywan-chungtsiang.top

Go:   time.Now()
来源：http://kft.sjlbkw.cn

Ruby: Time.now
来源：http://puc.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dto.bbcook.cn

[J02] 格式化输出
来源：http://rdf.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://est.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://shg.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wbl.zhixingplan.top

TS:   d.toISOString()
来源：http://rqt.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pbb.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dit.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnf.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ojn.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://xnf.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fyw.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://apm.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://orh.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://ufb.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://inx.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ucb.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://iic.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hhw.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://pzn.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nca.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://orb.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eec.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vyj.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dcb.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://stm.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://scz.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://txk.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://mdt.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://hpo.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sgf.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uzk.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rcv.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://vkp.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://euv.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://tns.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pdq.snrcjt.cn

[J06] 计算两时间之差
来源：http://nez.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://ksk.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://tmb.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rie.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eiy.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lxb.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://mfx.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://vuy.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://mgy.fengsongda.top

[J07] 比较两个日期
来源：http://xoq.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ztv.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vsj.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ykh.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://lcm.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izd.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ctz.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://rhj.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://zly.hfpthk.cn

[J08] 提取年月日与星期
来源：http://kwa.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oaq.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hki.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wnc.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tlh.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cak.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ewf.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oob.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iug.pycfn.com

[J09] 时区处理
来源：http://ago.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jhb.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vrh.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hpg.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qyi.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://scm.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qoh.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zrf.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jim.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://mlb.andypj.xyz


<!-- 参考信息 -->