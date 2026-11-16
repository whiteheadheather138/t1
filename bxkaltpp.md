代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://uii.smart0.xyz

Ruby: obj.instance_variables
来源：http://hax.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://wcn.haohaochexian.top

================================================================================
来源：http://pan.daria6918.cn

H. 异常与错误处理
来源：http://dpz.yvedp.cn

================================================================================
来源：http://nvh.nwbrower.top

[H01] try / catch 基础
来源：http://bnn.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xma.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ulk.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zpv.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wpj.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cog.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://imx.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://edj.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://emc.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://kbe.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://xih.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zqs.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hqc.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pby.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://kdu.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://tsk.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mcr.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vaj.gogol.net.cn

[H03] 主动抛出异常
来源：http://tdh.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://czx.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lsm.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://pik.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://qam.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxi.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohp.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nao.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://qui.wangdashe.top

[H04] 自定义异常类型
来源：http://alt.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://ewk.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://gsf.hammf.cn

JS:   class MyError extends Error {}
来源：http://fxg.cheryme.top

TS:   class MyError extends Error {}
来源：http://vgr.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://qry.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ttg.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://dvb.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://oau.jinqigufen.top

[H05] 捕获特定类型
来源：http://koy.smart0.xyz

Py:   except ValueError as e:
来源：http://tgr.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kfu.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://jqb.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://bcf.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://iqs.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ouq.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://ynd.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cnj.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://klv.fengsongda.top

Py:   value = d.get("k") or default
来源：http://tjr.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://lcs.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://gtr.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://lgy.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hev.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dsj.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://oow.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://gqa.jyoumei.cn

[H07] 断言
来源：http://wcr.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://rma.smart0.xyz

PHP:  assert($x > 0);
来源：http://vrb.yj20258.top

JS:   console.assert(x > 0);
来源：http://cji.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://yqt.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://lff.hysaishi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lkr.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://mbh.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://qeu.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://rcw.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://bda.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xmw.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://wzt.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sgh.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ffb.cucudq.cn

Go:   err.Error()
来源：http://cgl.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://dmz.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://hcm.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://qbv.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nuh.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lee.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dgj.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://drl.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxk.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cjn.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://tfg.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xta.bjfxy.top

[H10] 资源自动释放
来源：http://mgp.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://thi.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uaj.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sds.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oze.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rnn.zdqjudy.top

Go:   defer f.Close()
来源：http://fzy.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pbs.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rcy.yj202588.top

================================================================================
来源：http://gwm.xziqi.cn

I. 正则表达式
来源：http://bma.yj202588.top

================================================================================
来源：http://ovz.zdbjq.cn

[I01] 判断是否匹配
来源：http://zai.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vsa.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nio.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://yft.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://iep.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hvb.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://och.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://hew.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yfm.tian-w.cn

[I02] 提取所有匹配
来源：http://nvc.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://fbh.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://szl.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fvh.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://gxe.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xsl.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gyv.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://qoy.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tkp.zhoulong.xyz

[I03] 提取捕获分组
来源：http://usj.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dca.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://feh.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cho.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://imb.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mnm.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://syx.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hcf.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhb.shanyushiyangtech.top

[I04] 正则替换
来源：http://jwh.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://asl.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oqg.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://qrj.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://qma.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://ydl.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bdq.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://idp.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tdz.jyoumei.cn

[I05] 按正则拆分
来源：http://qas.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ggo.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mqb.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://rfd.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://soy.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://chw.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dvz.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://eyj.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xff.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gbx.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vds.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://djd.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://olx.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oce.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tnc.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qcf.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mmh.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hco.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://qkc.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pea.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dty.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxi.gogol.net.cn

TS:   /error/gim
来源：http://opp.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xdu.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zbf.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://qhh.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pwy.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://knv.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://son.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpw.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://htv.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rjh.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cai.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qul.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vnv.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://djj.shanyushiyangtech.top

================================================================================
来源：http://emb.cashguo.top

J. 日期与时间
来源：http://sud.yongpay.top

================================================================================
来源：http://uke.jqgufenzy.top

[J01] 获取当前时间
来源：http://szb.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cve.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://krc.yj20258.top

JS:   new Date();  Date.now()
来源：http://aeu.52xcode.cn

TS:   new Date();  Date.now()
来源：http://uxq.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ids.pengpengdd.cyou

Go:   time.Now()
来源：http://exg.bjfxy.top

Ruby: Time.now
来源：http://fze.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dbi.yongpay.top

[J02] 格式化输出
来源：http://cad.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wol.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://asd.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dgz.feifeiyinyue.top

TS:   d.toISOString()
来源：http://lpw.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kqh.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kws.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyv.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ukf.fehbvm.com

[J03] 字符串解析为日期
来源：http://bqu.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gfl.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nwg.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://yke.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://lug.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rmc.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hiq.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://bwr.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxg.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://epw.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://egf.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pda.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://osh.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uxy.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qvk.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iac.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://guo.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gar.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://wgq.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://sxx.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xwr.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ucr.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tbt.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://ahx.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://azp.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://txj.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://oui.yuxming.cn

[J06] 计算两时间之差
来源：http://dpw.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://kcj.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://hzf.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gkq.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mff.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://gow.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://geq.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://ndy.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://xsf.iojbl.cn

[J07] 比较两个日期
来源：http://inu.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://boi.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://brk.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wea.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hmn.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://opz.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ugb.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uqd.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://kxy.jyoumei.cn

[J08] 提取年月日与星期
来源：http://qwt.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hmt.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pjd.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://afq.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zid.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://non.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://puf.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cgx.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pqq.quarkkingdee.top

[J09] 时区处理
来源：http://lco.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://haq.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cke.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bgg.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://auv.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://siy.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gmd.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xva.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrq.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://gyq.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dzz.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rky.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uiv.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vdi.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rhv.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zsi.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzw.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uml.ydzc1.top

================================================================================
来源：http://haf.zhiwuduotai.top

K. JSON 与序列化
来源：http://nlm.sysykeji.top

================================================================================
来源：http://djx.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://ize.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dbn.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://glz.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://fsz.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://spj.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lzv.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://ren.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kou.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nyd.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://pbv.sxryk.cn

Py:   json.loads(s)
来源：http://fjr.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://alh.bjfxy.top

JS:   JSON.parse(s)
来源：http://ihv.jqgfzy.top

TS:   JSON.parse(s)
来源：http://uyp.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://piw.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://xef.nwbrower.top

Ruby: JSON.parse(s)
来源：http://xku.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://duu.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://bqt.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbz.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iic.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kem.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://keh.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pxo.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cah.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://isz.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lql.fktsv.cn

[K04] 读取 JSON 文件
来源：http://pnn.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mqc.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yge.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aii.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ljx.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jaw.xuanzx.com


<!-- 参考信息 -->