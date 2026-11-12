代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://rfh.yj20258888.top

Ruby: obj.instance_variables
来源：http://qpr.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://dvd.jinqigfzy.top

================================================================================
来源：http://cao.yonumen.top

H. 异常与错误处理
来源：http://gsr.xinyue.icu

================================================================================
来源：http://rlk.cheryme.top

[H01] try / catch 基础
来源：http://jgq.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qsx.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vel.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://poj.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rzd.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwq.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://trb.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://esq.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nnh.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://wjp.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://zvg.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://plc.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mau.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mtx.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://lej.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bjf.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tfl.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bff.ctjpmb.com

[H03] 主动抛出异常
来源：http://idh.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://nds.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pyi.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://zzj.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://cnb.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pvr.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ypu.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bcv.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://rql.smart0.xyz

[H04] 自定义异常类型
来源：http://ish.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://dpw.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://yqa.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://xaz.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://hbs.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://squ.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ihy.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://jnq.yj20258.top

C#:   class MyException : Exception {}
来源：http://qgu.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://zor.dianchejie.cn

Py:   except ValueError as e:
来源：http://aos.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://duq.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://emq.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://rdk.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://aay.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://idr.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://anr.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rcc.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://ekk.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://orr.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://vbd.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bjy.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://nwy.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fxb.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://occ.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://jgg.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://plz.52xcode.cn

[H07] 断言
来源：http://hxa.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://ieo.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://mvl.hnqzz.top

JS:   console.assert(x > 0);
来源：http://imd.52xcode.cn

TS:   console.assert(x > 0);
来源：http://bnp.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://rxg.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kag.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://olo.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://xxz.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://bzb.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://fap.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ugb.jinqigufen.top

JS:   e.message;  e.stack
来源：http://wsm.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tsd.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ugl.xylfe.cn

Go:   err.Error()
来源：http://smf.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://rto.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://lsx.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://lbc.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nlz.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ost.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jjt.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ljv.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xqu.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lgf.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://uvz.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://azk.fengsongda.top

[H10] 资源自动释放
来源：http://pya.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ecq.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hwo.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kxr.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cto.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.sysykeji.top

Go:   defer f.Close()
来源：http://gyv.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://atf.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://quq.sjlbkw.cn

================================================================================
来源：http://som.birdmap.top

I. 正则表达式
来源：http://qzb.ehwqpu.com

================================================================================
来源：http://eey.yuanzhike.top

[I01] 判断是否匹配
来源：http://xux.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uts.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://mhe.cashguo.top

JS:   /\d+/.test(s)
来源：http://eln.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://qhc.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gqq.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tzb.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://drr.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gnp.yuanzhike.top

[I02] 提取所有匹配
来源：http://aem.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://yxc.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zbr.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wku.havefunace.top

TS:   s.match(/\d+/g)
来源：http://qrg.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://asi.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qiy.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://yup.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sys.svipenyu.cn

[I03] 提取捕获分组
来源：http://eiw.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mup.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdj.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vwd.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://umr.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rlo.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ljz.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qbm.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdw.jyoumei.cn

[I04] 正则替换
来源：http://sik.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bmy.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohe.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nnn.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://aje.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://clz.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pgp.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eml.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ssy.nanxuanxn.top

[I05] 按正则拆分
来源：http://orv.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pge.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nnp.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://nng.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://xah.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://hwl.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nln.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://oow.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgs.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yep.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qdf.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xxy.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvx.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkc.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzz.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bbc.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bwg.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://upj.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://zqo.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rjg.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mpo.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qcd.wangdashe.top

TS:   /error/gim
来源：http://fup.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fxm.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pxk.sweek.top

Ruby: s.scan(/error/i)
来源：http://ctj.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xin.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://sxa.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vgb.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://weh.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wom.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aga.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lpz.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yvu.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nzo.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eaq.xuetiantiany.cn

================================================================================
来源：http://aah.cashguo.top

J. 日期与时间
来源：http://djj.zdbjq.cn

================================================================================
来源：http://etc.ybcxt.top

[J01] 获取当前时间
来源：http://jpq.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bte.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdk.vehdjk.com

JS:   new Date();  Date.now()
来源：http://tbd.hnqzz.top

TS:   new Date();  Date.now()
来源：http://odb.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://okb.52xcode.cn

Go:   time.Now()
来源：http://htb.ppjwa.cn

Ruby: Time.now
来源：http://gad.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://htd.fanxiaobao.xyz

[J02] 格式化输出
来源：http://whw.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hve.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lvq.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rnj.shangyingyoupin.top

TS:   d.toISOString()
来源：http://ytz.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tcu.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zni.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jeu.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jct.jiagoushi.top

[J03] 字符串解析为日期
来源：http://ehd.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ekg.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://grk.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://cel.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://gwm.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://yqw.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yyn.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://xgc.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://llm.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://fdc.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zxb.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://taa.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lbj.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ulr.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dfy.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://soh.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmo.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://frc.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://btc.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://gky.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vgc.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pra.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://den.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://ydf.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lpu.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://sgx.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kgs.chenzaomai.com

[J06] 计算两时间之差
来源：http://kue.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://nrd.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://ewv.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hcp.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rwk.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://amx.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://nlj.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://xni.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://wbr.hywenlv.cn

[J07] 比较两个日期
来源：http://fav.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://qiv.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofh.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ztm.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://bzj.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mzn.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ofj.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dpp.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://rfi.nwbrower.top

[J08] 提取年月日与星期
来源：http://ujl.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gsq.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwx.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vyi.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpz.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dbh.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vpq.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ord.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zfn.jlsjyb.cn

[J09] 时区处理
来源：http://pyg.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jny.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ehj.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcm.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://drb.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tcb.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgw.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eih.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://adk.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://hdu.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sah.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aty.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rrj.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://shs.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nvr.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rhy.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zcx.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rkk.zhoulong.xyz

================================================================================
来源：http://vgz.guowangkeji.top

K. JSON 与序列化
来源：http://akg.jlsjyb.cn

================================================================================
来源：http://qml.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://bnc.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zsy.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aln.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://ayq.havefunace.top

TS:   JSON.stringify(obj)
来源：http://rpr.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jjy.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://jku.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://igs.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yfu.yonumen.top

[K02] JSON 字符串转对象
来源：http://nji.gogol.net.cn

Py:   json.loads(s)
来源：http://puq.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wnn.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://mpn.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://rzb.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yyt.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://wjm.tarul.cn

Ruby: JSON.parse(s)
来源：http://law.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://opx.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://neg.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fdv.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zcf.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://izn.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eua.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ofh.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpp.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mpb.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uld.52xcode.cn

[K04] 读取 JSON 文件
来源：http://mas.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zkb.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fex.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ahc.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgo.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qwi.hnqzz.top


<!-- 参考信息 -->