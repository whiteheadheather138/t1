代发 wailian999

H. 异常与错误处理
来源：http://qve.nanxinkj.top

================================================================================
来源：http://dkx.yongpay.top

[H01] try / catch 基础
来源：http://tdb.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cyv.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://owt.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://toq.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqf.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vtk.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qoj.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://req.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cfo.sxryk.cn

[H02] finally / ensure 收尾
来源：http://kja.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://zgo.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://abb.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://cjh.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fzt.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://okj.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oon.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://yre.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://qak.tanke756.top

[H03] 主动抛出异常
来源：http://gll.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://hth.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uax.havefunace.top

JS:   throw new Error("错误信息");
来源：http://key.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://zfc.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://spg.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://von.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://snh.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://vmy.gogol.net.cn

[H04] 自定义异常类型
来源：http://rvs.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://xtu.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://hxr.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://moj.tarul.cn

TS:   class MyError extends Error {}
来源：http://bbj.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://ofd.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zpe.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://qzw.hesvh.cn

C#:   class MyException : Exception {}
来源：http://xcz.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://soe.yvedp.cn

Py:   except ValueError as e:
来源：http://thg.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oge.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://xzy.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://czp.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://git.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://utf.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://tji.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fud.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://zdy.fzhhl.top

Py:   value = d.get("k") or default
来源：http://kna.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://spj.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://asm.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ycs.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://shi.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qrg.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://vdy.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://add.wangshuangyany.cn

[H07] 断言
来源：http://rvy.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://ilj.cucudq.cn

PHP:  assert($x > 0);
来源：http://iao.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://slq.havefunace.top

TS:   console.assert(x > 0);
来源：http://sqm.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://pob.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pnr.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gyl.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://kfj.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://nqz.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://jwg.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mdv.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://nrr.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zcl.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jiv.quarkkingdee.top

Go:   err.Error()
来源：http://pjo.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://fkg.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://xqj.cdnleiting.top

[H09] 带错误码的异常
来源：http://ifp.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qnl.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pud.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dlr.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://icu.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://son.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gpy.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://bvi.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ymz.sufxvd.cn

[H10] 资源自动释放
来源：http://zyo.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sqn.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mjk.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zet.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nsa.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ssj.hnqzz.top

Go:   defer f.Close()
来源：http://has.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ptz.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nzi.xuanzx.com

================================================================================
来源：http://svo.jlsjyb.cn

I. 正则表达式
来源：http://swa.guowangkeji.top

================================================================================
来源：http://vvg.c1oappe.top

[I01] 判断是否匹配
来源：http://ebm.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iiz.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tnn.guannengcc.top

JS:   /\d+/.test(s)
来源：http://rwr.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://qwk.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://txe.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mdh.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://szj.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qic.smart0.xyz

[I02] 提取所有匹配
来源：http://lzi.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://xzi.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aqa.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tnb.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://lvg.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jqy.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qrl.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://ssw.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sub.yfazqb.com

[I03] 提取捕获分组
来源：http://ukg.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tds.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://inb.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ogl.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gqk.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://axk.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lox.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mdx.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fac.ydzc1.top

[I04] 正则替换
来源：http://prm.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mwh.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://txf.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tez.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yle.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xls.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vyu.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iqp.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qqy.fehbvm.com

[I05] 按正则拆分
来源：http://llr.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ukq.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cgq.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://wsf.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://dtr.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://sdn.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://caj.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://jjw.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pch.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ess.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gvx.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wes.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnp.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxj.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yqy.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ccl.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oha.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ibj.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://arl.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nms.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bod.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pva.iojbl.cn

TS:   /error/gim
来源：http://rrf.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oji.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ypn.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://rsv.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://usa.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://bfd.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://con.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wai.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bth.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbs.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mrj.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cnr.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tkb.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eks.meibo888.top

================================================================================
来源：http://fwb.hcnkem.com

J. 日期与时间
来源：http://gtt.daria6918.cn

================================================================================
来源：http://nwk.chenlongwang.top

[J01] 获取当前时间
来源：http://ooi.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrn.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://udd.xylfe.cn

JS:   new Date();  Date.now()
来源：http://cwv.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://gky.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://skb.cucudq.cn

Go:   time.Now()
来源：http://vdz.tian-w.cn

Ruby: Time.now
来源：http://wlp.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lji.jinqigufen.top

[J02] 格式化输出
来源：http://hyn.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgx.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qvq.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdn.bjfxy.top

TS:   d.toISOString()
来源：http://vgw.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://our.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zqp.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bcv.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qsu.fktsv.cn

[J03] 字符串解析为日期
来源：http://dhk.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fdv.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zre.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://kio.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://jvz.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ebw.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dxr.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://nsb.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbu.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://joe.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bjr.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jtp.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lzi.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://svm.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvl.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qaj.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://orh.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bgw.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://llq.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://fby.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hlp.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdj.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgc.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://riy.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vxl.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://abn.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://epb.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://ewh.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://ori.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://tey.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lic.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vat.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://afc.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://gbz.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://eqy.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://glc.vehdjk.com

[J07] 比较两个日期
来源：http://bzv.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://pux.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://szq.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hza.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fml.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zfp.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwl.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://izs.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://rne.uphjek.com

[J08] 提取年月日与星期
来源：http://qsx.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hxu.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sfr.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wdp.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iko.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ojk.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://okr.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lsg.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dew.shuidangran.top

[J09] 时区处理
来源：http://dii.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iox.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vdt.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adz.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggg.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://urj.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mtv.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aws.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sef.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://xlf.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zgs.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdm.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wie.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ogh.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ngc.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kzt.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uoh.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oyl.shangyingyoupin.top

================================================================================
来源：http://aci.zhoulong.xyz

K. JSON 与序列化
来源：http://ver.shuidangran.top

================================================================================
来源：http://cqv.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://ayo.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ghv.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sch.yj202588.top

JS:   JSON.stringify(obj)
来源：http://nag.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://dpk.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygh.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://hxl.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nst.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://clg.tanke756.top

[K02] JSON 字符串转对象
来源：http://rql.fzhhl.top

Py:   json.loads(s)
来源：http://kjj.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hxy.zycfv.cn

JS:   JSON.parse(s)
来源：http://nox.meibo888.top

TS:   JSON.parse(s)
来源：http://lou.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kmm.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://yqm.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://abn.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sos.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://wuq.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://toy.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pgz.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uov.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://avg.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fia.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ibl.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://exb.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qge.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://gan.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://znc.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jau.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gom.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvm.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qyq.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://owi.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ntn.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jyx.316326.xyz

[K05] 深拷贝对象
来源：http://nce.yj20258888.top


<!-- 参考信息 -->