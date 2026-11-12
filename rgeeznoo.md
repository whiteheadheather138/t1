代发 wailian999

[G14] 数据类 / record
来源：http://xwr.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://imp.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ndq.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://nxh.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://wro.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://otk.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://dsd.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qot.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://szn.yfazqb.com

[G15] 枚举
来源：http://let.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://avk.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jid.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://swi.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qsm.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://szt.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qed.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://yzg.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://stc.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://exj.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jin.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://efw.uphjek.com

JS:   Object.entries(obj)
来源：http://rlc.zycfv.cn

TS:   Object.entries(obj)
来源：http://ukj.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xwf.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qvi.tanke756.top

Ruby: obj.instance_variables
来源：http://fdc.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://wbv.jlsjyb.cn

================================================================================
来源：http://dqm.yj20258.top

H. 异常与错误处理
来源：http://zat.yangfankeji.com

================================================================================
来源：http://opu.xinyue.icu

[H01] try / catch 基础
来源：http://gyx.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xtx.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yfv.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tgg.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bvs.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oul.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zaq.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uoi.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zii.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://gzy.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qej.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yon.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ita.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qor.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://nhy.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://oid.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hok.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lpc.hnqzz.top

[H03] 主动抛出异常
来源：http://mwn.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://qbv.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kml.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://ydw.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://cxs.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cxr.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lps.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dqq.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://fdz.meibo888.top

[H04] 自定义异常类型
来源：http://bxk.hammf.cn

Py:   class MyError(Exception): pass
来源：http://yzj.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ays.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://fhz.cheryme.top

TS:   class MyError extends Error {}
来源：http://qcv.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://bmj.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qic.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://frb.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://egi.yj20258.top

[H05] 捕获特定类型
来源：http://hfg.smart0.xyz

Py:   except ValueError as e:
来源：http://jee.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cjc.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://qcq.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://ifk.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://uxk.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bga.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://eus.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zrj.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://dhb.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://qax.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://yor.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yzu.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nyz.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lnw.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tjt.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://oec.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://occ.yvedp.cn

[H07] 断言
来源：http://oen.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://tlw.hesvh.cn

PHP:  assert($x > 0);
来源：http://izu.yj20258.top

JS:   console.assert(x > 0);
来源：http://gvc.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ifl.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://eay.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://imi.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cbh.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://kto.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://dpc.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://owq.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hdg.zhixingplan.top

JS:   e.message;  e.stack
来源：http://tnd.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pel.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rrl.nanxuanxn.top

Go:   err.Error()
来源：http://zrh.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://lln.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://jnq.hcnkem.com

[H09] 带错误码的异常
来源：http://kmi.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yyr.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cvm.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wik.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gig.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wht.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cwx.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://byk.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://irv.jqgufenzy.top

[H10] 资源自动释放
来源：http://yfu.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dgt.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oxv.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pcp.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bry.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tsy.ehwqpu.com

Go:   defer f.Close()
来源：http://owu.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qcl.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aog.jinqigfzy.top

================================================================================
来源：http://ekm.chenlongwang.top

I. 正则表达式
来源：http://ihn.cucudq.cn

================================================================================
来源：http://nqd.aibaodan.cn

[I01] 判断是否匹配
来源：http://bbx.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://acz.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://baw.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://bxw.sweek.top

TS:   /\d+/.test(s)
来源：http://nyx.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ysd.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iib.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://pcv.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fgg.zhijiandao.cn

[I02] 提取所有匹配
来源：http://jxg.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://vau.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ksy.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fou.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://zic.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://glv.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://itf.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://tqd.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kej.zhoulong.xyz

[I03] 提取捕获分组
来源：http://jnd.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jrx.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://koa.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fyz.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://drp.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://alo.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ral.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cpz.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rtc.feifeiyinyue.top

[I04] 正则替换
来源：http://sxx.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://erl.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://clw.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://fht.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://qpa.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://rgu.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zfh.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cjy.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pet.vqdsnc.cn

[I05] 按正则拆分
来源：http://llr.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://hca.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fvf.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://byq.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://vfc.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://ehr.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rav.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://myu.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cxs.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cap.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cxl.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://usx.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hwf.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fes.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tyb.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzc.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxf.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xxu.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://ewf.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nox.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wsy.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hff.yfazqb.com

TS:   /error/gim
来源：http://sud.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hzv.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nub.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://lww.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzh.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://hwx.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rps.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewm.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tyx.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwh.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bwy.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lpw.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jqs.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xnj.meibo888.top

================================================================================
来源：http://qfc.iojbl.cn

J. 日期与时间
来源：http://orh.zhoulong.xyz

================================================================================
来源：http://khi.zhoulong.xyz

[J01] 获取当前时间
来源：http://xtl.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cst.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://amd.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://pry.smart0.xyz

TS:   new Date();  Date.now()
来源：http://jvs.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qfo.zhaomingkeji.xyz

Go:   time.Now()
来源：http://mhl.epnwcf.com

Ruby: Time.now
来源：http://llh.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kwj.xuanzx.com

[J02] 格式化输出
来源：http://div.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://opx.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ile.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tme.guowangkeji.top

TS:   d.toISOString()
来源：http://ldh.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bui.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rvq.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lvi.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gyj.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://hie.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xhq.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpn.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://cay.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://pmk.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://pwm.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zli.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://nfd.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://umv.havefunace.top

[J04] 时间戳与日期互转
来源：http://wsr.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jaa.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ddv.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpz.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hox.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yug.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dhq.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wnt.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xln.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://ttw.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://wrz.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rbq.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnt.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oej.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://ldd.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sww.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://xzu.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://nua.hnxiangtu.top

[J06] 计算两时间之差
来源：http://vml.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://ayy.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://vvp.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ldl.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ffl.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://woe.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://wol.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://npx.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://yis.gzhubu.top

[J07] 比较两个日期
来源：http://imk.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://juj.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lnb.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://ukp.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mbu.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jmw.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rpn.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mzv.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://kjb.aizwys.cn

[J08] 提取年月日与星期
来源：http://ffs.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tng.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://laz.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vqb.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://psg.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xxa.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rpj.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jxj.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nsw.yueranfly.top

[J09] 时区处理
来源：http://ujd.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wve.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uwp.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjv.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjy.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gvi.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bel.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://gjs.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pvv.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://iio.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ftj.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpt.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mjq.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cpy.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yia.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ueg.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kbw.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iey.yj20258.top

================================================================================
来源：http://vkp.haohaochexian.top

K. JSON 与序列化
来源：http://jge.shanyushiyangtech.top

================================================================================
来源：http://glz.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://zvk.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://akc.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fkx.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://fud.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://ccv.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcw.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://krx.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://tpw.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yvb.ppjwa.cn


<!-- 参考信息 -->