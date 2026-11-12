代发 wailian999

H. 异常与错误处理
来源：http://svk.gaohongyu789.top

================================================================================
来源：http://ash.zhengqikj.top

[H01] try / catch 基础
来源：http://enq.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ncu.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqj.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rmt.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lgo.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hgg.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mkn.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tqv.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dei.yj20258.top

[H02] finally / ensure 收尾
来源：http://dyw.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://aty.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gvf.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eln.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yjp.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rww.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uzf.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://icr.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ely.yuxming.cn

[H03] 主动抛出异常
来源：http://lle.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://gye.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://otf.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://wfu.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://aqm.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ktp.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rfm.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://tuj.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://akt.tian-w.cn

[H04] 自定义异常类型
来源：http://iax.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://zox.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://azq.guannengcc.top

JS:   class MyError extends Error {}
来源：http://fep.bbcook.cn

TS:   class MyError extends Error {}
来源：http://otz.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://glk.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xcy.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://tmk.tanke756.top

C#:   class MyException : Exception {}
来源：http://nzx.jqgufenzy.top

[H05] 捕获特定类型
来源：http://bcw.zhixingplan.top

Py:   except ValueError as e:
来源：http://yeg.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wyi.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://rep.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://eav.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://ele.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wdq.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://rue.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xwp.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://ehr.52xcode.cn

Py:   value = d.get("k") or default
来源：http://qmq.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://fbb.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xww.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://etr.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrn.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cil.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://dps.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://mjz.jinyuanbaomall.cn

[H07] 断言
来源：http://yud.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://bkm.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://bar.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://lxn.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://tux.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://zyi.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mie.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://zxw.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://brk.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://tge.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://scz.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zjp.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://mse.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pkw.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uxt.zhiwuduotai.top

Go:   err.Error()
来源：http://wij.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://ndx.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://rqg.bbcook.cn

[H09] 带错误码的异常
来源：http://rtu.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wjd.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://lzp.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ntu.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ljo.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pax.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jee.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zyw.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fqg.xinyue.icu

[H10] 资源自动释放
来源：http://kch.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xoe.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fee.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://szx.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fyi.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjn.yangfankeji.com

Go:   defer f.Close()
来源：http://bwq.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jxj.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dqa.tianlin.xyz

================================================================================
来源：http://ebk.yonumen.top

I. 正则表达式
来源：http://hmh.hongshengwenyu.top

================================================================================
来源：http://azx.hesvh.cn

[I01] 判断是否匹配
来源：http://gkq.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qpd.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://itu.xziqi.cn

JS:   /\d+/.test(s)
来源：http://guo.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://cuo.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lwf.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uyp.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://ddl.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxt.sufxvd.cn

[I02] 提取所有匹配
来源：http://eti.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://tpe.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ptb.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yzf.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://the.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wrj.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qmb.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://jfv.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uej.cdnleiting.top

[I03] 提取捕获分组
来源：http://uvp.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mfq.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ejv.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ryi.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://udo.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kkp.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dxf.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vgl.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yyx.zhixingplan.top

[I04] 正则替换
来源：http://iic.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://plp.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bgw.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://nsa.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dyd.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://glu.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tsp.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fhy.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yom.shangyingyoupin.top

[I05] 按正则拆分
来源：http://cvx.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dop.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qpu.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://ckw.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://ftt.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://vvh.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ykt.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oza.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gbm.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kgh.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wba.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iws.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpp.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvm.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cjr.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rxr.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gpp.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vif.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://qva.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uvj.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zks.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gjr.nanxuanxn.top

TS:   /error/gim
来源：http://bdu.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tya.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ehu.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://ntf.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tvx.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://aek.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hib.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogv.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xli.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://edm.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxg.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cue.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bpk.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nkc.jinqigufen.top

================================================================================
来源：http://pba.svipenyu.cn

J. 日期与时间
来源：http://nww.jinqigufen.top

================================================================================
来源：http://hjc.epnwcf.com

[J01] 获取当前时间
来源：http://trm.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rox.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aof.yueranfly.top

JS:   new Date();  Date.now()
来源：http://tfc.havefunace.top

TS:   new Date();  Date.now()
来源：http://yvj.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://goy.zdqjudy.top

Go:   time.Now()
来源：http://wfr.yuanzhike.top

Ruby: Time.now
来源：http://iqe.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bwb.sjlbkw.cn

[J02] 格式化输出
来源：http://pju.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwx.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ydo.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bxl.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://cbp.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zoc.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hem.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xtt.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jpy.haohaochexian.top

[J03] 字符串解析为日期
来源：http://vog.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://por.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kth.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://fse.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://dbi.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jpj.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://acn.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://tot.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qmx.bjfxy.top

[J04] 时间戳与日期互转
来源：http://ppu.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://igz.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bhr.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lwl.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qus.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wdh.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gpu.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgr.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqd.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://shi.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://ngt.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://sgy.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pef.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozn.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ejp.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lml.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://kqk.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vdn.yongpay.top

[J06] 计算两时间之差
来源：http://iun.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://lcl.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://hfg.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mol.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vbv.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://ptc.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://fzw.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://wpl.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://qyd.ybcxt.top

[J07] 比较两个日期
来源：http://dgi.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://dfo.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://trz.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://vao.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://txf.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pcz.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uea.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://juv.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://jdf.bjfxy.top

[J08] 提取年月日与星期
来源：http://ibo.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qxk.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zgi.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://psq.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qcf.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ftu.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hyr.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dwp.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uhv.jianghu66.top

[J09] 时区处理
来源：http://kqt.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gel.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qeh.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pav.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbh.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ean.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rhl.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lro.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uzt.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://tfe.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wft.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jls.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mks.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dyq.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://czn.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bip.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cbr.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bjm.snrcjt.cn

================================================================================
来源：http://dko.zhixingplan.top

K. JSON 与序列化
来源：http://nac.yuanzhike.top

================================================================================
来源：http://hfe.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://dvw.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zdl.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://skv.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://gfo.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://bdb.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ukf.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://eab.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://hry.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nlo.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://imj.zhixingplan.top

Py:   json.loads(s)
来源：http://ywy.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dhk.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://klu.0kj1m.cn

TS:   JSON.parse(s)
来源：http://nwk.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pdr.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://hla.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://rjn.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mkc.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://ntc.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ecc.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gji.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xtm.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jcw.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://upp.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqb.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tqp.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gtv.ybcxt.top

[K04] 读取 JSON 文件
来源：http://lqx.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gvf.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://odt.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://txg.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pue.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fgl.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yjy.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wra.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nnt.gogol.net.cn

[K05] 深拷贝对象
来源：http://qui.hnxiangtu.top


<!-- 参考信息 -->