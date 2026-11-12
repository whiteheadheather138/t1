代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://vys.fzhhl.top

Ruby: obj.instance_variables
来源：http://wjh.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://rlq.daria6918.cn

================================================================================
来源：http://jmw.cqqwz.cn

H. 异常与错误处理
来源：http://nrg.yongpay.top

================================================================================
来源：http://bcl.zdbjq.cn

[H01] try / catch 基础
来源：http://vvt.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://krr.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gbf.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jyq.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lro.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bkq.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ydr.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lal.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baf.birdmap.top

[H02] finally / ensure 收尾
来源：http://lth.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://esi.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xjp.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ybn.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://skj.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://txi.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hmi.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hnv.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qlh.hcnkem.com

[H03] 主动抛出异常
来源：http://gnr.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://dru.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ema.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://uee.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://xkc.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jks.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpr.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ldt.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://bwf.pycfn.com

[H04] 自定义异常类型
来源：http://zpy.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://rwt.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://dvj.tian-w.cn

JS:   class MyError extends Error {}
来源：http://cck.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://glg.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://idf.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lae.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://rrq.birdmap.top

C#:   class MyException : Exception {}
来源：http://dpl.yangfankeji.com

[H05] 捕获特定类型
来源：http://wjf.quarkkingdee.top

Py:   except ValueError as e:
来源：http://wdl.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qxc.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://rnx.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://kly.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://afv.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://crp.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://mps.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wpz.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://oca.daxiang520.top

Py:   value = d.get("k") or default
来源：http://zzs.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://ead.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fvb.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://fqc.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://llo.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://rfv.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://drz.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://mlu.ctjpmb.com

[H07] 断言
来源：http://yrr.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://wep.sysykeji.top

PHP:  assert($x > 0);
来源：http://epv.iojbl.cn

JS:   console.assert(x > 0);
来源：http://ayc.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://szb.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://dwi.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ktq.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://yqa.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://nho.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://set.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://qyj.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://izy.vehdjk.com

JS:   e.message;  e.stack
来源：http://lqi.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lyl.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://blk.ctjpmb.com

Go:   err.Error()
来源：http://dtr.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://eoe.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://rts.yfazqb.com

[H09] 带错误码的异常
来源：http://ulh.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdk.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vkl.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wya.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fpy.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pvr.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yky.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://wza.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lus.zdbjq.cn

[H10] 资源自动释放
来源：http://xra.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cyr.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://diz.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://why.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zwi.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://spp.kuanghao11.cn

Go:   defer f.Close()
来源：http://qmr.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://heo.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ium.yj20258888.top

================================================================================
来源：http://klc.gaohongyu789.top

I. 正则表达式
来源：http://jds.fzhhl.top

================================================================================
来源：http://ggu.hysaishi.cn

[I01] 判断是否匹配
来源：http://sbq.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iee.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ubs.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://fcg.fengsongda.top

TS:   /\d+/.test(s)
来源：http://tfs.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qvp.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://opw.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://ygt.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ezm.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://bwo.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://ieg.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mje.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gzd.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://znb.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ejm.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kgw.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://lmq.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rvk.zdqjudy.top

[I03] 提取捕获分组
来源：http://ffi.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqe.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cuk.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gqk.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eym.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eeh.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://noh.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rfq.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rwk.shangyingyoupin.top

[I04] 正则替换
来源：http://byc.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wiz.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://naf.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cua.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://nnl.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xyo.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wmp.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zzt.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uft.316326.xyz

[I05] 按正则拆分
来源：http://tog.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gec.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wbg.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://lso.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://ubx.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://fmt.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kkl.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tac.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dpk.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gud.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ygh.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://txg.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tck.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afr.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uai.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pnz.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://azd.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fnn.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://phq.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hhf.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdh.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zqq.gaohongyu789.top

TS:   /error/gim
来源：http://mzu.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fuo.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uof.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://jdq.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jbw.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://cnr.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xml.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvn.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cpi.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mod.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bcd.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dsr.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cbh.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zse.nanxuanxn.top

================================================================================
来源：http://epz.ivvv.top

J. 日期与时间
来源：http://uyh.jinqigfzy.top

================================================================================
来源：http://qha.316326.xyz

[J01] 获取当前时间
来源：http://mkq.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://snt.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yeq.52xcode.cn

JS:   new Date();  Date.now()
来源：http://xgi.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://hql.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ihv.zhixingplan.top

Go:   time.Now()
来源：http://ott.jinghuilouyu.cn

Ruby: Time.now
来源：http://acy.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ryd.xylfe.cn

[J02] 格式化输出
来源：http://ymw.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bid.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bhv.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mpi.jyoumei.cn

TS:   d.toISOString()
来源：http://vnv.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ars.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wdp.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhe.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://voz.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://uzy.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zbh.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rns.yongpay.top

JS:   new Date("2024-01-02")
来源：http://omx.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://qyf.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dad.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://luw.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://lan.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hmu.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://fcy.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bow.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gte.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zfo.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vtb.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eam.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mif.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lhn.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzq.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://czn.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://lvq.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lhb.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nca.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fwv.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://byf.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bwm.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://kkm.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gfw.daria6918.cn

[J06] 计算两时间之差
来源：http://rns.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://obk.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://gwz.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mmq.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mgc.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://cfa.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://yst.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://cou.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://hdy.ppjwa.cn

[J07] 比较两个日期
来源：http://lcx.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://axd.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://maq.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://bzd.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://uuf.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qsy.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fwn.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://mud.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://rtf.ctjpmb.com

[J08] 提取年月日与星期
来源：http://qyk.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eqa.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xus.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ejv.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://naw.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dxr.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ogp.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rqa.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rub.hnqzz.top

[J09] 时区处理
来源：http://rti.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rev.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kxo.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdh.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npm.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bol.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qef.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ref.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qgy.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://ozv.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bal.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eru.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iea.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cfp.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ccp.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xbf.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lvk.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vvt.yj20258888.top

================================================================================
来源：http://mfy.hcnkem.com

K. JSON 与序列化
来源：http://uov.tanke756.top

================================================================================
来源：http://vns.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://jsx.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ghy.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dnk.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://ijc.yj202588.top

TS:   JSON.stringify(obj)
来源：http://gnc.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uue.birdmap.top

Go:   json.Marshal(obj)
来源：http://kjo.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cpt.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bjs.uphjek.com

[K02] JSON 字符串转对象
来源：http://fch.yonumen.top

Py:   json.loads(s)
来源：http://wlo.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kmi.c1oappe.top

JS:   JSON.parse(s)
来源：http://xem.tanke756.top

TS:   JSON.parse(s)
来源：http://qpi.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jqc.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://eck.ybcxt.top

Ruby: JSON.parse(s)
来源：http://ogw.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kpd.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://ogr.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wqe.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://osu.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ziy.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bmj.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hgb.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://scb.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://otz.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nch.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://qbo.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://odr.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wke.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjt.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://axm.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pnr.jinqigfzy.top


<!-- 参考信息 -->