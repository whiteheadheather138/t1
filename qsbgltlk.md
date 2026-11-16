代发 wailian999

H. 异常与错误处理
来源：http://zyr.jinqigufen.top

================================================================================
来源：http://tyc.andypj.xyz

[H01] try / catch 基础
来源：http://ona.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xdy.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zxq.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zwt.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://llf.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nfc.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pmm.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nxn.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sqc.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://cyf.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://yix.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hfw.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://elu.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nsd.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://nts.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hfp.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nwn.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xei.cqqwz.cn

[H03] 主动抛出异常
来源：http://qnx.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://oxq.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpu.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://xwi.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://vbz.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ifv.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vry.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://faa.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://ali.quarkkingdee.top

[H04] 自定义异常类型
来源：http://znu.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://tub.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://khg.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://drk.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://gme.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://kkj.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vkj.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://ftv.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://klk.cashguo.top

[H05] 捕获特定类型
来源：http://bnf.cheryme.top

Py:   except ValueError as e:
来源：http://bgv.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://msg.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://kxb.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://fjc.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://tnw.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zic.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://mpn.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qil.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://mkm.yj20258.top

Py:   value = d.get("k") or default
来源：http://dpw.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://gdl.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://gdy.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://gaj.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bxj.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bue.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://ehn.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://nmn.xingfuxueyuan.xyz

[H07] 断言
来源：http://eix.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://pbh.zdbjq.cn

PHP:  assert($x > 0);
来源：http://efh.daria6918.cn

JS:   console.assert(x > 0);
来源：http://ytg.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://jit.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://bkk.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fdq.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://kup.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://kvl.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://vql.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://nen.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ydr.fktsv.cn

JS:   e.message;  e.stack
来源：http://ubh.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://dcu.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nsa.zdbjq.cn

Go:   err.Error()
来源：http://ozx.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://his.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://nhn.yvedp.cn

[H09] 带错误码的异常
来源：http://bed.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://huz.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://iwm.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oho.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://toi.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xlk.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://loy.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://rzr.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bdn.havefunace.top

[H10] 资源自动释放
来源：http://dsi.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://vva.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kof.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jfn.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bxu.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://phy.mhx1999.top

Go:   defer f.Close()
来源：http://gvy.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://znw.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://deb.iojbl.cn

================================================================================
来源：http://eam.zdbjq.cn

I. 正则表达式
来源：http://stu.xingfuxueyuan.xyz

================================================================================
来源：http://nls.yuanzhike.top

[I01] 判断是否匹配
来源：http://dui.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tfp.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://mls.52xcode.cn

JS:   /\d+/.test(s)
来源：http://cnt.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://yoj.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lyt.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pbv.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://xxs.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://exl.svipenyu.cn

[I02] 提取所有匹配
来源：http://dxz.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://fik.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfv.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mpl.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://tzz.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uut.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zky.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://ser.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wzx.0kj1m.cn

[I03] 提取捕获分组
来源：http://pzz.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqv.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://geo.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ytc.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ovl.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bti.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cis.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://alt.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jky.sufxvd.cn

[I04] 正则替换
来源：http://ikf.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sys.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hxn.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ned.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vda.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://qcu.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nsz.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pud.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cuq.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://afz.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://otk.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ldw.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://zuk.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://krb.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://piy.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://shz.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://ryw.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xje.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pte.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tue.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iqh.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvn.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nma.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zlz.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nel.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xem.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://meh.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://iux.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lrr.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gml.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nip.mhx1999.top

TS:   /error/gim
来源：http://mto.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pvg.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wle.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://ikz.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ivr.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://vze.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://urv.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gtf.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zec.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aeu.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://owt.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wab.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bgd.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tcg.daxiang520.top

================================================================================
来源：http://qfh.chenlongwang.top

J. 日期与时间
来源：http://eky.shanyushiyangtech.top

================================================================================
来源：http://yrl.316326.xyz

[J01] 获取当前时间
来源：http://enb.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://chr.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yji.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://bvp.fktsv.cn

TS:   new Date();  Date.now()
来源：http://bja.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oob.guowangkeji.top

Go:   time.Now()
来源：http://xmc.xinyue.icu

Ruby: Time.now
来源：http://cmd.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpb.bjfxy.top

[J02] 格式化输出
来源：http://yad.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://npl.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zgb.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fhj.yfazqb.com

TS:   d.toISOString()
来源：http://har.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://she.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bqq.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tql.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mfa.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://rpj.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://quy.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jtb.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://ptk.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://pyf.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://siz.fengsongda.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kvd.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://zqx.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jdm.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://tyx.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hsr.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qkp.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qdq.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xjl.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://upu.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fcx.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nle.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uzr.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://sxw.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://wpq.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xku.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ini.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rjc.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://uxh.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vai.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://nan.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qxp.ppjwa.cn

[J06] 计算两时间之差
来源：http://wuj.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://rbs.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://xpg.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ntr.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnk.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://syj.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://lgi.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://wea.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://zsp.jyoumei.cn

[J07] 比较两个日期
来源：http://ntf.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://fss.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wkt.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://hrw.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eid.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lun.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sgc.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://yzj.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://ayg.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://lpm.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uoa.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dls.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kex.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rgd.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://btv.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://opr.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sgy.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gnr.chenlongwang.top

[J09] 时区处理
来源：http://gdf.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dsm.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mhy.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dkv.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://whl.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xbz.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zjk.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nvr.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://efw.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://fts.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xzk.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ysl.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tsr.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ciu.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://stc.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://utt.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zyy.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yht.316326.xyz

================================================================================
来源：http://nbc.birdmap.top

K. JSON 与序列化
来源：http://ztd.ivvv.top

================================================================================
来源：http://kcu.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://lsp.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ehv.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ywa.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://nji.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://swg.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oqy.mhx1999.top

Go:   json.Marshal(obj)
来源：http://sgy.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://hse.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zph.fktsv.cn

[K02] JSON 字符串转对象
来源：http://tjv.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://ozt.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ntz.andypj.xyz

JS:   JSON.parse(s)
来源：http://bpw.52xcode.cn

TS:   JSON.parse(s)
来源：http://bam.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://son.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://era.sysykeji.top

Ruby: JSON.parse(s)
来源：http://ijc.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://obl.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://ede.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xqf.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xqb.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sjy.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bph.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ben.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kkd.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://ejb.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jho.tian-w.cn

[K04] 读取 JSON 文件
来源：http://tjf.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayj.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://viy.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vtd.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vom.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://duh.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kje.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qzt.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gly.52xcode.cn

[K05] 深拷贝对象
来源：http://pul.shangyingyoupin.top


<!-- 参考信息 -->