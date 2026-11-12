代发 wailian999

PHP:  get_object_vars($obj);
来源：http://qes.tarul.cn

JS:   Object.entries(obj)
来源：http://nto.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://djp.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qeo.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rmt.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://nix.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://thb.shzxlz.cn

================================================================================
来源：http://ixs.xuetiantiany.cn

H. 异常与错误处理
来源：http://lra.sysykeji.top

================================================================================
来源：http://pul.hnqzz.top

[H01] try / catch 基础
来源：http://cyw.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jgo.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lzv.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vlq.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ioo.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tyx.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uxq.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://etl.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jjy.zycfv.cn

[H02] finally / ensure 收尾
来源：http://fuc.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://pel.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qmv.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qtw.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rro.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://uga.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jod.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://upe.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mfi.jlsjyb.cn

[H03] 主动抛出异常
来源：http://dse.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://gnl.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gdy.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://poo.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://mdn.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hsx.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qoj.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ywo.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://prs.aizwys.cn

[H04] 自定义异常类型
来源：http://qvd.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://vzg.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://yid.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://rxm.yuxming.cn

TS:   class MyError extends Error {}
来源：http://bif.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://wko.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nne.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://pyd.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://ifp.hywenlv.cn

[H05] 捕获特定类型
来源：http://psm.dashuyun.cn

Py:   except ValueError as e:
来源：http://lqt.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mnv.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://ctj.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://yno.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://bxi.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qpg.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://rlx.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jns.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://fei.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://woc.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://qxa.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://acm.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hcf.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zku.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ucx.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://kmp.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://vnt.jiagoushi.top

[H07] 断言
来源：http://qlo.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://jkh.316326.xyz

PHP:  assert($x > 0);
来源：http://jxe.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://nsp.fzhhl.top

TS:   console.assert(x > 0);
来源：http://nbi.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://hfy.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nww.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vhs.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://gna.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://dvv.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://aog.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lwx.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://faj.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwg.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qad.jinqigufen.top

Go:   err.Error()
来源：http://cdb.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://ulu.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://ban.chenlongwang.top

[H09] 带错误码的异常
来源：http://hfu.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://plt.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jfv.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ksz.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uxv.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uvw.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zzq.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://exc.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://udd.ehwqpu.com

[H10] 资源自动释放
来源：http://akt.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kbg.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sis.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jbi.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://joq.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dnd.xziqi.cn

Go:   defer f.Close()
来源：http://jor.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cgv.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kpw.birdmap.top

================================================================================
来源：http://aeg.ywan-chungtsiang.top

I. 正则表达式
来源：http://pcu.chenlongwang.top

================================================================================
来源：http://vzb.zhengqikj.top

[I01] 判断是否匹配
来源：http://vsp.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wdd.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://xse.yfazqb.com

JS:   /\d+/.test(s)
来源：http://tun.cheryme.top

TS:   /\d+/.test(s)
来源：http://ult.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yjl.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bgv.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://pal.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sww.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://hib.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://xta.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cnd.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uuk.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://izs.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axg.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pom.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://dae.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lvx.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://rrv.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xsy.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xvx.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lnb.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ryc.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mni.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ple.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://img.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lug.zhaomingkeji.xyz

[I04] 正则替换
来源：http://mjp.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ism.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://elc.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://cyo.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nnf.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cnc.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vdd.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://fct.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lpp.pengpengdd.cyou

[I05] 按正则拆分
来源：http://mlb.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aym.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhe.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://pbe.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://gpd.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://gkw.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kbn.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://wyp.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eaf.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vqd.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lvj.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mmt.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ddd.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sis.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dou.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rrg.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vgd.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://far.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://usa.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vrn.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tsy.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nzn.ivvv.top

TS:   /error/gim
来源：http://odc.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xvi.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hgg.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://zuy.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iud.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ayx.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vli.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jsq.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xza.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xrf.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://wih.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bge.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xdq.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xlp.aibaodan.cn

================================================================================
来源：http://peu.dashuyun.cn

J. 日期与时间
来源：http://ccv.ybcxt.top

================================================================================
来源：http://gdg.dianchejie.cn

[J01] 获取当前时间
来源：http://mvi.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dvb.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yif.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://dls.52xcode.cn

TS:   new Date();  Date.now()
来源：http://cgr.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dqo.jinyuanbaomall.cn

Go:   time.Now()
来源：http://dhc.gogol.net.cn

Ruby: Time.now
来源：http://nev.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lhz.xinyue.icu

[J02] 格式化输出
来源：http://lwz.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhl.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://apa.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ako.yueranfly.top

TS:   d.toISOString()
来源：http://vxw.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sxw.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uek.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zat.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xis.fktsv.cn

[J03] 字符串解析为日期
来源：http://dbi.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pxm.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lqv.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://hpf.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://rmw.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ufv.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://npz.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://wmc.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fms.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://ufx.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yiu.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zam.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dvs.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://swx.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://opn.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nao.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vsa.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://loy.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://ioh.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://aep.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://asa.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yxg.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aup.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://kqq.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eza.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://hww.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://ytn.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://hql.yj202588.top

Py:   (end - start).total_seconds()
来源：http://lve.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://emd.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gmk.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxl.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://yog.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://bmp.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://ijt.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://zdy.guannengcc.top

[J07] 比较两个日期
来源：http://rcl.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://mwm.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gry.cdnleiting.top

JS:   d1.getTime() < d2.getTime()
来源：http://wwd.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://sfz.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://trz.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wjk.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mjh.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dlt.daria6918.cn

[J08] 提取年月日与星期
来源：http://eqi.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vmy.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://epi.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gsg.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kbv.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://czu.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cto.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uwe.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qcc.ydzc1.top

[J09] 时区处理
来源：http://gya.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mok.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivy.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edl.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lha.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hsp.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vby.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oma.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pkc.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://dwi.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qgj.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uff.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ogv.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lbu.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://agw.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pob.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqp.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nsg.yj20258.top

================================================================================
来源：http://hfz.cucudq.cn

K. JSON 与序列化
来源：http://njn.zhixingplan.top

================================================================================
来源：http://rsk.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://zyn.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yzd.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vlz.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://scl.birdmap.top

TS:   JSON.stringify(obj)
来源：http://pfx.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jus.cheryme.top

Go:   json.Marshal(obj)
来源：http://pcf.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cnb.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://llz.meibo888.top

[K02] JSON 字符串转对象
来源：http://ehc.xuanzx.com

Py:   json.loads(s)
来源：http://puz.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lcc.bbcook.cn

JS:   JSON.parse(s)
来源：http://ehj.yuxming.cn

TS:   JSON.parse(s)
来源：http://kgg.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dis.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://jjt.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://ijv.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wrp.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://hgr.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cbj.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ohf.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ptx.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://sbz.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kkd.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://awt.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://tps.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ivt.hcnkem.com

[K04] 读取 JSON 文件
来源：http://aky.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqj.hysaishi.cn


<!-- 参考信息 -->