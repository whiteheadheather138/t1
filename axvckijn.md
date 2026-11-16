代发 wailian999

[G14] 数据类 / record
来源：http://stl.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lom.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://azv.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rfo.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://tgw.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://ygz.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://wfy.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ktd.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://tnu.xingfuxueyuan.xyz

[G15] 枚举
来源：http://fui.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vzl.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://djg.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ggu.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://osw.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://mes.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ddv.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://jqr.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ome.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://few.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhw.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://yat.epnwcf.com

JS:   Object.entries(obj)
来源：http://fmt.xylfe.cn

TS:   Object.entries(obj)
来源：http://ixz.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hrh.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rmu.52xcode.cn

Ruby: obj.instance_variables
来源：http://teu.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://wix.xuetiantiany.cn

================================================================================
来源：http://ktf.tianlin.xyz

H. 异常与错误处理
来源：http://jzq.feifeiyinyue.top

================================================================================
来源：http://axk.cashguo.top

[H01] try / catch 基础
来源：http://rzk.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sfd.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dzc.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mhz.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xfs.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bug.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vnb.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xaz.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tyv.sysykeji.top

[H02] finally / ensure 收尾
来源：http://cac.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jvx.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xgp.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://skh.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qne.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://ont.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mku.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zpc.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yqk.nanxuanxn.top

[H03] 主动抛出异常
来源：http://pbm.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://omt.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cgp.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://ttm.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://hfr.yfazqb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://mea.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jhi.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mkq.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://ebn.epnwcf.com

[H04] 自定义异常类型
来源：http://agj.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://yra.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qgk.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://lpw.pycfn.com

TS:   class MyError extends Error {}
来源：http://zkh.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://osh.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ccx.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://kqk.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://msl.mhx1999.top

[H05] 捕获特定类型
来源：http://isi.52xcode.cn

Py:   except ValueError as e:
来源：http://cfi.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qfr.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://qeu.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://brf.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://qev.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://liw.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://rci.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dvl.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://hkj.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://tow.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://the.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oue.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://ems.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xuz.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ftb.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://umh.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://rfi.svipenyu.cn

[H07] 断言
来源：http://pfr.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://yhz.xziqi.cn

PHP:  assert($x > 0);
来源：http://hmj.daxiang520.top

JS:   console.assert(x > 0);
来源：http://imz.sxryk.cn

TS:   console.assert(x > 0);
来源：http://dgr.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://ker.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dga.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lwi.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://qcf.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://hmr.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://rkh.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zct.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://lwo.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yze.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bwi.vehdjk.com

Go:   err.Error()
来源：http://eay.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://fjn.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://zqs.kuanghao11.cn

[H09] 带错误码的异常
来源：http://nmd.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ymg.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://qpj.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pzc.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lsj.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dcl.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vtp.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hps.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lbw.guowangkeji.top

[H10] 资源自动释放
来源：http://lyn.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://acm.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zws.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qwa.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ktx.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mro.xuetiantiany.cn

Go:   defer f.Close()
来源：http://zvk.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iwg.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lci.nwbrower.top

================================================================================
来源：http://irn.pycfn.com

I. 正则表达式
来源：http://rat.xylfe.cn

================================================================================
来源：http://sdy.uphjek.com

[I01] 判断是否匹配
来源：http://hyk.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sic.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://thl.gzhubu.top

JS:   /\d+/.test(s)
来源：http://jnj.yj20258.top

TS:   /\d+/.test(s)
来源：http://ohu.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lqu.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rch.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://aqn.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xvo.tanke756.top

[I02] 提取所有匹配
来源：http://ukt.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://suz.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jzj.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dpj.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://zez.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://syb.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mik.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://ili.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mqw.fengsongda.top

[I03] 提取捕获分组
来源：http://kkx.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xru.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jco.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://giv.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jar.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://syw.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hta.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ajp.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kcb.yj20258.top

[I04] 正则替换
来源：http://fck.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iiu.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ndu.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zpe.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://dqw.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://lzv.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vui.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jou.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xql.tian-w.cn

[I05] 按正则拆分
来源：http://tqz.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ulf.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vvp.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://fjj.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://qmm.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://doh.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zbw.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://blo.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dlu.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kgf.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://syd.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bsu.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyc.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ohz.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cmq.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wyj.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wvm.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gyo.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://sxe.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iwg.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://neg.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xfo.bbcook.cn

TS:   /error/gim
来源：http://hgt.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tmt.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wnu.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://vnk.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pyp.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wrb.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ewi.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lxh.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxh.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://thz.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hpv.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mgc.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://seo.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzz.gotoacloud.top

================================================================================
来源：http://lwm.fengsongda.top

J. 日期与时间
来源：http://iyi.sweek.top

================================================================================
来源：http://dse.andypj.xyz

[J01] 获取当前时间
来源：http://msa.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nrr.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bct.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://boq.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://jft.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lmw.pengpengdd.cyou

Go:   time.Now()
来源：http://jek.9152youxi.cn

Ruby: Time.now
来源：http://eoc.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qpl.fktsv.cn

[J02] 格式化输出
来源：http://mnx.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwf.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gry.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://own.wangdashe.top

TS:   d.toISOString()
来源：http://tbl.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vce.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qem.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nrt.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xmp.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://tsj.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uio.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hia.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://nct.yj202588.top

TS:   new Date("2024-01-02")
来源：http://yit.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://ffa.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rex.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://ebm.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pau.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://qhd.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eqd.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xcb.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qpd.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qps.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ikx.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fup.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wuw.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://giz.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://izk.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://ljq.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bhz.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbj.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hiu.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://xnu.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zuj.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://prx.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://mfb.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://mir.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://mjh.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://kid.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://crb.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bvt.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vif.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://mty.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://div.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://uvq.bjfxy.top

[J07] 比较两个日期
来源：http://paa.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://cap.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gsr.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://jkm.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://tbj.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xss.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://crh.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://fqg.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://zns.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://fzm.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ffj.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ynt.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gek.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hto.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://esw.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ghi.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xbr.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vkl.yvedp.cn

[J09] 时区处理
来源：http://yaj.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hce.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vfv.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjt.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vef.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wyg.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://upa.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://epf.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qnq.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://bre.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rmt.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aks.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qcq.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sdr.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nno.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hdn.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oad.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kbi.ydzc1.top

================================================================================
来源：http://kex.cdnleiting.top

K. JSON 与序列化
来源：http://nbt.shanyushiyangkeji.top

================================================================================
来源：http://lhn.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://mrc.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hxw.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aft.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://lal.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://igs.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eie.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://wnr.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xpd.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://lnp.wangshuangyany.cn


<!-- 参考信息 -->