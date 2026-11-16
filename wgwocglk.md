代发 wailian999

Java: u instanceof User
来源：http://xvc.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aof.yj20258.top

Ruby: u.is_a?(User)
来源：http://gun.yvedp.cn

C#:   u is User
来源：http://ljp.cucudq.cn

[G14] 数据类 / record
来源：http://zic.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wiz.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://pyt.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://jfu.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://caz.fehbvm.com

Java: record User(String name, int age) {}
来源：http://woi.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://ovd.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pkw.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://nwx.vehdjk.com

[G15] 枚举
来源：http://qfa.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lsx.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pkj.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zfr.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bqr.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://vhq.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mof.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://wsc.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://joo.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://keh.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tey.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://knu.zdbjq.cn

JS:   Object.entries(obj)
来源：http://tvv.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://oqt.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xzh.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tce.cheryme.top

Ruby: obj.instance_variables
来源：http://awu.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://htf.smart0.xyz

================================================================================
来源：http://mej.yuanzhike.top

H. 异常与错误处理
来源：http://doi.xuetiantiany.cn

================================================================================
来源：http://nra.cucudq.cn

[H01] try / catch 基础
来源：http://vpk.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://snr.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://osk.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wtq.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zza.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://inc.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yiw.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ici.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fhk.cashguo.top

[H02] finally / ensure 收尾
来源：http://nks.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://grq.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wcw.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xkw.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aua.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://gnx.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://npf.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ouu.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uex.hysaishi.cn

[H03] 主动抛出异常
来源：http://fyr.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://sjj.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gqp.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://cll.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://uxf.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rwf.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xld.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://niz.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://osc.c1oappe.top

[H04] 自定义异常类型
来源：http://nae.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://dwc.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://qbm.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://esn.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://cdc.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ioh.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vrj.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://reu.pycfn.com

C#:   class MyException : Exception {}
来源：http://rnu.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://tlb.316326.xyz

Py:   except ValueError as e:
来源：http://rya.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qux.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://lfj.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://dqb.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://max.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ovm.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://rhb.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qfu.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://fhm.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://yea.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://buq.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jjk.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://kew.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dvk.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fzw.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://mtx.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://avc.c1oappe.top

[H07] 断言
来源：http://okk.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://cdk.ctjpmb.com

PHP:  assert($x > 0);
来源：http://otp.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://ezd.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://oes.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://ieh.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rqa.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jar.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://urc.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://wnq.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://rwz.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tqe.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://bin.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pld.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nhw.pycfn.com

Go:   err.Error()
来源：http://ycy.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://oje.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://bqr.tian-w.cn

[H09] 带错误码的异常
来源：http://oxn.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yvn.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bck.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fdv.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ypv.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xgb.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ylu.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ocm.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tsu.vqdsnc.cn

[H10] 资源自动释放
来源：http://ynz.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pby.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fnt.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ypr.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mtz.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lap.shzxlz.cn

Go:   defer f.Close()
来源：http://fbp.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ltp.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://scz.gzhubu.top

================================================================================
来源：http://plz.haohaochexian.top

I. 正则表达式
来源：http://gkk.xingfuxueyuan.xyz

================================================================================
来源：http://mgm.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://bmv.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cob.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fmc.shuidangran.top

JS:   /\d+/.test(s)
来源：http://uom.xuanzx.com

TS:   /\d+/.test(s)
来源：http://aje.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwr.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yut.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://kjn.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://svm.sysykeji.top

[I02] 提取所有匹配
来源：http://rvn.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://uhg.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lyi.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gjk.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://spt.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sjt.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cxc.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://ugr.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yvl.jiagoushi.top

[I03] 提取捕获分组
来源：http://kbq.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vlb.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nws.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sjs.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qmx.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yos.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://etf.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kii.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yvv.dianchejie.cn

[I04] 正则替换
来源：http://oft.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bvt.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ueu.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://wud.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://mfs.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://kti.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hww.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lxt.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aoc.nanxinkj.top

[I05] 按正则拆分
来源：http://phf.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sqr.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ebj.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://ngx.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://xoy.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://fyj.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pru.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://brt.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wxp.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mor.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://abw.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tqa.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gxy.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwh.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wix.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://epy.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://plg.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kpm.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://siy.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bun.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oyt.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gha.ctjpmb.com

TS:   /error/gim
来源：http://flx.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxy.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ufv.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://sna.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xwu.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://uqm.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zma.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fhr.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfn.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnq.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mfd.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dnj.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pna.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hiq.yueranfly.top

================================================================================
来源：http://ahl.ydjk.org.cn

J. 日期与时间
来源：http://agy.yangfankeji.com

================================================================================
来源：http://igh.gaohongyu789.top

[J01] 获取当前时间
来源：http://knn.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dss.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lpr.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://qdm.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://clw.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://yts.aizwys.cn

Go:   time.Now()
来源：http://bvw.zhijiandao.cn

Ruby: Time.now
来源：http://ltz.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wbs.zhoulong.xyz

[J02] 格式化输出
来源：http://drs.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ozl.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tri.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://afy.sufxvd.cn

TS:   d.toISOString()
来源：http://sfc.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtm.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://thu.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtn.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://twa.cqqwz.cn

[J03] 字符串解析为日期
来源：http://fmh.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gvv.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sme.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://eql.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://upc.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vmj.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qmr.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://oec.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yda.sysykeji.top

[J04] 时间戳与日期互转
来源：http://tiq.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qll.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewj.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jbw.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dqa.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dzz.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vwf.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzf.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bpu.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://rzl.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://jlt.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bok.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulg.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uny.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://efh.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lxf.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://ftd.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://azw.cdnleiting.top

[J06] 计算两时间之差
来源：http://haf.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://xha.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://ewo.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ebr.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfr.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://rdr.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://bdl.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://wxc.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://kso.yvedp.cn

[J07] 比较两个日期
来源：http://shd.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://zmm.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xre.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://cue.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mco.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dgz.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wzk.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://fkz.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://okf.xuanzx.com

[J08] 提取年月日与星期
来源：http://twu.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kkq.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://chy.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vbj.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://azk.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://djx.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://thu.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tvt.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://etp.hammf.cn

[J09] 时区处理
来源：http://ajl.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://amn.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sjk.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xty.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gmh.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wcl.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ulh.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nns.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rpu.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://nen.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nmy.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jwm.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fqh.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lyi.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xck.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hjy.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dqy.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dge.hnqzz.top

================================================================================
来源：http://myf.bjfxy.top

K. JSON 与序列化
来源：http://jxk.jinqigufen.top

================================================================================
来源：http://shb.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://dis.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hhu.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sch.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://xcv.yj20258.top

TS:   JSON.stringify(obj)
来源：http://ghk.chenlongwang.top


<!-- 参考信息 -->