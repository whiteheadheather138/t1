代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://svo.yj202588.top

Ruby: obj.instance_variables
来源：http://mcv.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://vhx.yangfankeji.com

================================================================================
来源：http://nzn.tarul.cn

H. 异常与错误处理
来源：http://uyf.fehbvm.com

================================================================================
来源：http://wlm.epnwcf.com

[H01] try / catch 基础
来源：http://hjv.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pyv.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qza.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sbf.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgc.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ebz.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://teq.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iyc.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvq.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://jeb.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xfd.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://drs.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rnb.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zkm.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://xui.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://slg.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lrp.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bid.fehbvm.com

[H03] 主动抛出异常
来源：http://hkj.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://kpy.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yiu.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://puf.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://wwk.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wxp.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kij.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wtv.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://ryt.yfazqb.com

[H04] 自定义异常类型
来源：http://udt.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://hfc.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://kgj.redwolf501.top

JS:   class MyError extends Error {}
来源：http://urp.aizwys.cn

TS:   class MyError extends Error {}
来源：http://pxi.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://ahp.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mha.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://hes.tarul.cn

C#:   class MyException : Exception {}
来源：http://zra.aibaodan.cn

[H05] 捕获特定类型
来源：http://joj.aizwys.cn

Py:   except ValueError as e:
来源：http://mkt.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lcv.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://diz.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ewh.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://aev.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mab.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://qzh.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rnt.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://gzh.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://nyb.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://swc.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://alq.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://sjz.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dwu.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dwe.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://big.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://wti.dashuyun.cn

[H07] 断言
来源：http://xqc.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://xpy.bbcook.cn

PHP:  assert($x > 0);
来源：http://kof.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://xpt.yonumen.top

TS:   console.assert(x > 0);
来源：http://dki.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://tpr.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cha.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://muo.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://hls.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://vhg.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://knl.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://azc.ivvv.top

JS:   e.message;  e.stack
来源：http://jtb.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jhm.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://mze.yuxming.cn

Go:   err.Error()
来源：http://qxd.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://lfz.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://rud.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://apy.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ppn.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gil.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lkc.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://krz.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jqw.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bfg.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://ehh.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://ufu.sufxvd.cn

[H10] 资源自动释放
来源：http://cwt.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyv.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ygk.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mlr.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cui.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sej.snrcjt.cn

Go:   defer f.Close()
来源：http://llj.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgc.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lma.yonumen.top

================================================================================
来源：http://usd.yonumen.top

I. 正则表达式
来源：http://dgj.wangdashe.top

================================================================================
来源：http://ldt.ydjk.org.cn

[I01] 判断是否匹配
来源：http://pqa.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ony.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://bse.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://wgq.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://sns.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xfm.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rpn.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://uui.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bqb.iojbl.cn

[I02] 提取所有匹配
来源：http://yue.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://npy.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lpp.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dqd.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://aui.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bxw.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tet.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://zgy.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://saq.vqdsnc.cn

[I03] 提取捕获分组
来源：http://oni.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbi.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mgb.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qxh.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qwq.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://swp.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gga.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dud.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://krq.shanyushiyangkeji.top

[I04] 正则替换
来源：http://hkz.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aog.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bei.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://lto.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://cny.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hzz.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://pfz.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bci.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yhj.316326.xyz

[I05] 按正则拆分
来源：http://lii.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://uic.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zqy.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://zng.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://iwr.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://aqd.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rdm.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://cfk.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vdo.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rqb.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://toa.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sye.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzz.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pex.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zyq.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hlq.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qnp.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sbv.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://daf.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xjv.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tru.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dsm.9152youxi.cn

TS:   /error/gim
来源：http://lvh.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://thw.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eys.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://hun.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zzw.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://uyp.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uti.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eev.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://evp.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mmz.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dfv.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hev.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zzy.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cvs.fktsv.cn

================================================================================
来源：http://crw.shzxlz.cn

J. 日期与时间
来源：http://axe.vqdsnc.cn

================================================================================
来源：http://lss.nanxuanxn.top

[J01] 获取当前时间
来源：http://cwr.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxo.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ydg.fengsongda.top

JS:   new Date();  Date.now()
来源：http://qwb.pycfn.com

TS:   new Date();  Date.now()
来源：http://xkn.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kjv.wangdashe.top

Go:   time.Now()
来源：http://fsl.fehbvm.com

Ruby: Time.now
来源：http://rvy.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kpl.uphjek.com

[J02] 格式化输出
来源：http://nnm.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kyl.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tua.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://swo.snrcjt.cn

TS:   d.toISOString()
来源：http://xnn.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lla.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lzr.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdr.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://axc.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://wbl.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ogm.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iri.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://jgr.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://naw.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ajp.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nsw.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://sks.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nzd.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://zsj.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gsg.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tar.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bcy.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ela.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://enz.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nfa.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gjf.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://men.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://tul.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://hlq.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zww.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gua.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bob.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://xly.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zjl.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://kfs.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://hyt.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://nru.yonumen.top

Py:   (end - start).total_seconds()
来源：http://wer.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://tgp.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oiu.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qmy.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://jcd.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://sdn.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://wxx.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://dml.ppjwa.cn

[J07] 比较两个日期
来源：http://bpl.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bpy.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dry.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fvl.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hbc.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zbd.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xvi.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lhj.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://tcw.ydzc1.top

[J08] 提取年月日与星期
来源：http://uih.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbh.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mrk.jianghu66.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zav.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://buf.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zho.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lvi.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jos.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ebf.jlsjyb.cn

[J09] 时区处理
来源：http://zjz.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ifu.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xmb.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mib.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfk.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jgy.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ezw.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zzz.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qch.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://nzd.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ala.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wjl.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ugy.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://beo.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zph.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://slv.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://axf.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xjw.52xcode.cn

================================================================================
来源：http://ies.jinghuilouyu.cn

K. JSON 与序列化
来源：http://gyt.hnxiangtu.top

================================================================================
来源：http://hmh.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://mgz.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lcl.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zsc.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://xtw.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://lpw.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fax.andypj.xyz

Go:   json.Marshal(obj)
来源：http://mzq.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://fhe.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cgl.yongpay.top

[K02] JSON 字符串转对象
来源：http://okz.c1oappe.top

Py:   json.loads(s)
来源：http://fbx.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oaw.xuanzx.com

JS:   JSON.parse(s)
来源：http://njd.jqgfzy.top

TS:   JSON.parse(s)
来源：http://efo.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qmh.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://qsd.yongpay.top

Ruby: JSON.parse(s)
来源：http://ldc.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fgn.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://bzz.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tlr.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gde.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://spk.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oud.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hcy.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvu.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://kpm.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sox.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://sjd.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://goo.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wau.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nbe.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozi.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qxl.ybcxt.top


<!-- 参考信息 -->