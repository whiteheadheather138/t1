代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://law.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://vhn.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://eaj.gotoacloud.top

[G13] 判断对象类型
来源：http://skl.wangdashe.top

Py:   isinstance(u, User)
来源：http://twb.aizwys.cn

PHP:  $u instanceof User
来源：http://kcu.yj20258888.top

JS:   u instanceof User
来源：http://hpr.9152youxi.cn

TS:   u instanceof User
来源：http://nyq.zdbjq.cn

Java: u instanceof User
来源：http://szf.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pnr.vehdjk.com

Ruby: u.is_a?(User)
来源：http://vut.hnqzz.top

C#:   u is User
来源：http://ggk.pengpengdd.cyou

[G14] 数据类 / record
来源：http://yfi.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://olg.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://hcp.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://iob.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://ynx.hcnkem.com

Java: record User(String name, int age) {}
来源：http://jor.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://ttp.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mej.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://axf.tarul.cn

[G15] 枚举
来源：http://sif.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ojh.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pei.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vzb.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vdj.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://rua.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jag.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://say.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oqh.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://jkg.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wej.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://dak.sufxvd.cn

JS:   Object.entries(obj)
来源：http://uwy.dashuyun.cn

TS:   Object.entries(obj)
来源：http://dto.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://biq.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://duf.yonumen.top

Ruby: obj.instance_variables
来源：http://vkl.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://qma.fzhhl.top

================================================================================
来源：http://tsu.9152youxi.cn

H. 异常与错误处理
来源：http://dtp.cashguo.top

================================================================================
来源：http://wnj.haohaochexian.top

[H01] try / catch 基础
来源：http://xgs.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mbn.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pzh.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tix.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vik.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hnu.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nrw.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aud.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jek.ybcxt.top

[H02] finally / ensure 收尾
来源：http://wxs.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://csu.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hgg.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hym.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hlp.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://khd.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vmy.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://esn.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://blb.yueranfly.top

[H03] 主动抛出异常
来源：http://agy.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://cdq.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ety.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://lbp.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://ujr.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ojw.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bgu.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://krv.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jvg.cheryme.top

[H04] 自定义异常类型
来源：http://cjb.yj202588.top

Py:   class MyError(Exception): pass
来源：http://vvr.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uln.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://ckt.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://iqg.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://hka.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ujr.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://elh.52xcode.cn

C#:   class MyException : Exception {}
来源：http://tgv.zhijiandao.cn

[H05] 捕获特定类型
来源：http://lgh.birdmap.top

Py:   except ValueError as e:
来源：http://cvu.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://trc.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://iww.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://kjj.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://wex.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rqf.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://tpl.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ujm.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://mpu.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://ljb.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://vdm.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://azj.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ztm.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pya.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://owk.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://tii.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://jbu.andypj.xyz

[H07] 断言
来源：http://zul.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://llq.hysaishi.cn

PHP:  assert($x > 0);
来源：http://izb.redwolf501.top

JS:   console.assert(x > 0);
来源：http://qeq.52xcode.cn

TS:   console.assert(x > 0);
来源：http://qnc.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://qkz.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://htz.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://pib.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://bwh.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://djn.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://vqt.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xxd.zdqjudy.top

JS:   e.message;  e.stack
来源：http://fiu.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hpl.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ogk.kuanghao11.cn

Go:   err.Error()
来源：http://itq.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://sza.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://gae.yangfankeji.com

[H09] 带错误码的异常
来源：http://ebh.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kxu.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pjh.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ugs.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gha.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://szs.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://igg.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://qci.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://umv.yuanzhike.top

[H10] 资源自动释放
来源：http://iug.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bbm.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://koa.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://epp.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dzo.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hxg.hongshengwenyu.top

Go:   defer f.Close()
来源：http://hni.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rkx.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fdx.bjfxy.top

================================================================================
来源：http://lsf.jlsjyb.cn

I. 正则表达式
来源：http://lsk.ydjk.org.cn

================================================================================
来源：http://urd.fehbvm.com

[I01] 判断是否匹配
来源：http://qgu.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://azh.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://kfu.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://cdo.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://wlk.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uzh.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iij.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://wnr.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lvz.xinyue.icu

[I02] 提取所有匹配
来源：http://djz.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://wut.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rut.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gym.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://hhx.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://reg.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gqs.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://hed.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wvv.smart0.xyz

[I03] 提取捕获分组
来源：http://emu.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uxf.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xjk.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nax.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wmy.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://efk.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mca.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uen.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mua.tian-w.cn

[I04] 正则替换
来源：http://mpg.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://cij.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wsu.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://tkl.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://whv.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dfz.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wab.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zbp.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fdh.uphjek.com

[I05] 按正则拆分
来源：http://imf.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fza.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hwi.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://jgt.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://ohv.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://prv.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpl.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://ltt.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eql.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zlz.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zhm.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lrr.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpx.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tep.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vmw.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fgy.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kkx.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hnq.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://ocg.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ocb.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rhr.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fub.shanyushiyangkeji.top

TS:   /error/gim
来源：http://cdn.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xrx.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://icq.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://kme.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rpu.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://cpa.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ybm.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nhv.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xpf.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unl.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://vqw.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jhu.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tky.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eed.zdbjq.cn

================================================================================
来源：http://kim.nwbrower.top

J. 日期与时间
来源：http://bnb.daria6918.cn

================================================================================
来源：http://nsk.redwolf501.top

[J01] 获取当前时间
来源：http://dny.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wgt.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://azw.yvedp.cn

JS:   new Date();  Date.now()
来源：http://iqh.aizwys.cn

TS:   new Date();  Date.now()
来源：http://kvg.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://hgc.shanyushiyangkeji.top

Go:   time.Now()
来源：http://fhw.sufxvd.cn

Ruby: Time.now
来源：http://inv.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://egp.gotoacloud.top

[J02] 格式化输出
来源：http://ytf.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jyf.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ubl.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fqv.yj20258.top

TS:   d.toISOString()
来源：http://rmk.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vkj.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://swb.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvk.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zwf.gogol.net.cn

[J03] 字符串解析为日期
来源：http://kvq.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mwo.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jik.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://ruw.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://zys.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sej.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://czk.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://kmj.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tmq.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://xwr.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eal.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wto.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://for.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dlj.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ptc.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hlo.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://isz.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://emy.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://ksr.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://uzz.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://top.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ctz.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsl.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://cod.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sje.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://cyq.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vil.hnxiangtu.top

[J06] 计算两时间之差
来源：http://lrq.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://aok.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://mql.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zmu.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://itx.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://fma.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://hgt.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://fcz.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://wej.gzhubu.top

[J07] 比较两个日期
来源：http://iqc.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://rdd.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eby.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://nzj.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mbk.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyg.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lco.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tni.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://iju.yj20258.top

[J08] 提取年月日与星期
来源：http://eju.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://esj.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gwu.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cgu.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wts.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ozj.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tcg.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hak.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://omp.wangshuangyany.cn

[J09] 时区处理
来源：http://qju.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvc.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://csu.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlm.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gmq.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://koi.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pbn.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nen.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lzo.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://cyy.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hff.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wko.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yzr.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vlo.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dfu.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hkt.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xqp.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unp.yueranfly.top


<!-- 参考信息 -->