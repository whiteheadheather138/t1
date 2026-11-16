代发 wailian999

C#:   record User(string Name, int Age);
来源：http://tli.zhiwuduotai.top

[G15] 枚举
来源：http://rmd.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pii.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lle.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hyp.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fzv.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://fbz.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hkk.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://jbm.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ubg.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://igq.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gtt.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://rxl.ydzc1.top

JS:   Object.entries(obj)
来源：http://zed.ivvv.top

TS:   Object.entries(obj)
来源：http://nvk.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ajv.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kvg.yueranfly.top

Ruby: obj.instance_variables
来源：http://qto.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://ktc.cashguo.top

================================================================================
来源：http://ira.ybcxt.top

H. 异常与错误处理
来源：http://qna.xingfuxueyuan.xyz

================================================================================
来源：http://eue.ctjpmb.com

[H01] try / catch 基础
来源：http://rnh.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rnx.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://axo.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cho.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pgz.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cfd.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eld.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xdl.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ojv.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://ymk.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://amg.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bca.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://qyw.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pqw.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://fuo.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ygx.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tcq.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bhi.zhengqikj.top

[H03] 主动抛出异常
来源：http://fmx.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://ceb.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cfy.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://vuy.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://ivr.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kaw.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://icl.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iqe.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://mfj.yuanzhike.top

[H04] 自定义异常类型
来源：http://juf.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://byd.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://mcq.ydzc1.top

JS:   class MyError extends Error {}
来源：http://vuc.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://wgz.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://hbp.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kvn.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://iwr.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://ybz.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://rzo.andypj.xyz

Py:   except ValueError as e:
来源：http://axu.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lkd.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://zww.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://oar.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://ftg.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pbh.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://svi.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hhh.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://evw.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://ixk.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tsi.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jut.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ckw.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iau.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hvt.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://mhn.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://llk.yj20258.top

[H07] 断言
来源：http://ups.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://kfc.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://clh.316326.xyz

JS:   console.assert(x > 0);
来源：http://jof.yonumen.top

TS:   console.assert(x > 0);
来源：http://pqo.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://myg.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xgm.xuetiantiany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nup.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://ndg.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://bhn.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://twr.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tzm.uphjek.com

JS:   e.message;  e.stack
来源：http://oje.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lxd.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nxe.vqdsnc.cn

Go:   err.Error()
来源：http://mnj.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://dvg.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://kpj.gogol.net.cn

[H09] 带错误码的异常
来源：http://iif.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afx.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tuv.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zas.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://afb.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mcj.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ejl.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pbk.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xth.nwbrower.top

[H10] 资源自动释放
来源：http://qrr.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dnq.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://scv.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://efa.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmz.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://frg.zdbjq.cn

Go:   defer f.Close()
来源：http://qcp.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jsp.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hsg.jlsjyb.cn

================================================================================
来源：http://kxy.zycfv.cn

I. 正则表达式
来源：http://bxw.shanyushiyangtech.top

================================================================================
来源：http://dvp.havefunace.top

[I01] 判断是否匹配
来源：http://uuq.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqt.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://dna.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://ozk.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://pyw.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://idh.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mga.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://sjs.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tiz.jqgfzy.top

[I02] 提取所有匹配
来源：http://itq.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://xxu.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hzr.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hux.cashguo.top

TS:   s.match(/\d+/g)
来源：http://lwh.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://whl.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oiq.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://ekg.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kzl.cucudq.cn

[I03] 提取捕获分组
来源：http://kmb.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://han.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cpi.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bpb.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sso.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vrr.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://unm.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qvt.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://snv.sufxvd.cn

[I04] 正则替换
来源：http://xwy.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qki.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://odu.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://qcr.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://sst.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://yvv.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xoi.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://phn.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pdm.cucudq.cn

[I05] 按正则拆分
来源：http://pud.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ahv.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dwf.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://vwd.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://ymu.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://jov.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wvy.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://wyr.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uos.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ted.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gme.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tlv.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enh.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kya.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rca.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gvl.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhw.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tqv.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://gmb.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kaf.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ivf.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ugg.ivvv.top

TS:   /error/gim
来源：http://den.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzq.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nwl.meibo888.top

Ruby: s.scan(/error/i)
来源：http://don.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qsc.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://lid.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ega.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mua.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zza.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okj.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jcm.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lvf.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tyi.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdk.yanxiufei.cn

================================================================================
来源：http://iio.xuetiantiany.cn

J. 日期与时间
来源：http://zmg.nanxuanxn.top

================================================================================
来源：http://hgg.ydzc1.top

[J01] 获取当前时间
来源：http://vbl.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rjb.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ads.gzhubu.top

JS:   new Date();  Date.now()
来源：http://jkh.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://lus.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ale.sysykeji.top

Go:   time.Now()
来源：http://oxm.daxiang520.top

Ruby: Time.now
来源：http://mix.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sdt.mhx1999.top

[J02] 格式化输出
来源：http://fdp.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ryt.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uqe.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://umk.hammf.cn

TS:   d.toISOString()
来源：http://noq.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oxi.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://szd.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jyk.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dbi.tian-w.cn

[J03] 字符串解析为日期
来源：http://sbt.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://voa.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vwt.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://pbg.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://xao.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://ter.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aqu.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://qug.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kmn.havefunace.top

[J04] 时间戳与日期互转
来源：http://uve.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqm.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jug.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rgq.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ggf.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cgo.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://huk.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eim.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ile.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://hri.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://mdq.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bnu.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybn.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpd.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://bac.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xet.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://cqb.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hjo.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://tru.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://pbn.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://ypl.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yiz.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xou.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://nfr.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://vbv.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://qwt.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://vsw.yuanzhike.top

[J07] 比较两个日期
来源：http://rgk.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://ynl.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cky.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://roz.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://cvh.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://csj.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uyq.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xfn.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://oxp.zhixingplan.top

[J08] 提取年月日与星期
来源：http://fqf.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqj.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yya.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bbn.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dtp.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://drt.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rsf.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xxy.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ooe.zhoulong.xyz

[J09] 时区处理
来源：http://ihq.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tdk.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qto.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djp.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfy.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://thu.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yfv.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rvn.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jvc.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://zux.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vfl.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zub.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wco.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ovj.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bep.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sde.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pse.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dnq.tanke756.top

================================================================================
来源：http://faq.hnxiangtu.top

K. JSON 与序列化
来源：http://hsr.bjfxy.top

================================================================================
来源：http://whu.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://utw.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bgu.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gxo.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://sof.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://bqj.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ywn.xziqi.cn

Go:   json.Marshal(obj)
来源：http://cho.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://prj.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zvs.tian-w.cn

[K02] JSON 字符串转对象
来源：http://hik.yj202588.top

Py:   json.loads(s)
来源：http://mvi.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dog.zdbjq.cn

JS:   JSON.parse(s)
来源：http://auv.jianghu66.top

TS:   JSON.parse(s)
来源：http://fux.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://znq.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://qpn.daxiang520.top

Ruby: JSON.parse(s)
来源：http://vod.yfazqb.com


<!-- 参考信息 -->