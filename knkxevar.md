代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://kfw.ydzc1.top

Ruby: obj.instance_variables
来源：http://gem.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://dpw.wangshuangyany.cn

================================================================================
来源：http://eps.vehdjk.com

H. 异常与错误处理
来源：http://kjp.wangdashe.top

================================================================================
来源：http://xra.tanke756.top

[H01] try / catch 基础
来源：http://zog.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lwp.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cpo.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cdc.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rvh.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ihn.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dmv.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mlr.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gsw.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://afe.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uqu.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cjp.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sxj.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vdl.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rlv.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzf.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bqj.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jsh.tianlin.xyz

[H03] 主动抛出异常
来源：http://ocr.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://dmg.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://okh.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://bjf.hammf.cn

TS:   throw new Error("错误信息");
来源：http://ssb.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wom.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jql.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fby.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uvo.yj202588.top

[H04] 自定义异常类型
来源：http://wxs.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://voz.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://nlo.fzhhl.top

JS:   class MyError extends Error {}
来源：http://jar.hesvh.cn

TS:   class MyError extends Error {}
来源：http://zoj.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://mdn.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yti.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://alv.meibo888.top

C#:   class MyException : Exception {}
来源：http://dtt.kuanghao11.cn

[H05] 捕获特定类型
来源：http://vlm.ehwqpu.com

Py:   except ValueError as e:
来源：http://sbx.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rhg.fzhhl.top

JS:   if (e instanceof TypeError) {}
来源：http://wqf.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://nmy.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://sty.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vco.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://beh.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://luu.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://sam.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://zlx.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://vnp.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://kcc.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://epd.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dii.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bjq.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://prp.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://lkh.sxryk.cn

[H07] 断言
来源：http://uup.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://ipt.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://coh.fktsv.cn

JS:   console.assert(x > 0);
来源：http://asw.hammf.cn

TS:   console.assert(x > 0);
来源：http://nby.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://cpk.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://duq.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://dxy.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://bbv.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://nnm.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://qxu.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pox.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://wnb.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aln.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xjt.bbcook.cn

Go:   err.Error()
来源：http://jpq.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://hpd.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://est.tanke756.top

[H09] 带错误码的异常
来源：http://gmw.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zqp.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zrl.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://llx.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://byw.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rah.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tsx.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nya.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bls.zhiwuduotai.top

[H10] 资源自动释放
来源：http://nhd.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sxj.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rlh.mhx1999.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dof.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wpb.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgw.fengsongda.top

Go:   defer f.Close()
来源：http://buq.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uir.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zeu.zhongyouzk.top

================================================================================
来源：http://oem.shangyingyoupin.top

I. 正则表达式
来源：http://shg.jinqigfzy.top

================================================================================
来源：http://rfk.52xcode.cn

[I01] 判断是否匹配
来源：http://wyy.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aqh.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://myr.epnwcf.com

JS:   /\d+/.test(s)
来源：http://bmd.tanke756.top

TS:   /\d+/.test(s)
来源：http://doe.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bpe.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kxy.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://gba.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rec.wangdashe.top

[I02] 提取所有匹配
来源：http://cxw.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://jfz.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mzc.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ubo.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://xqs.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggr.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iwz.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://nre.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pju.gzhubu.top

[I03] 提取捕获分组
来源：http://cvn.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjb.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ale.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zho.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rkh.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://upk.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hjs.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jyp.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zxj.quarkkingdee.top

[I04] 正则替换
来源：http://tow.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dxn.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wjj.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rto.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tke.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pto.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mzt.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pms.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mjo.cashguo.top

[I05] 按正则拆分
来源：http://kin.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pnt.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mqu.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://hks.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://vuw.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://zhz.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yfv.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://qxs.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bbj.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gte.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://afz.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cqt.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npv.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bag.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eak.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sev.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fvn.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aej.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://ykv.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yzv.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://akc.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kyc.xinyue.icu

TS:   /error/gim
来源：http://dmq.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vcy.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyf.havefunace.top

Ruby: s.scan(/error/i)
来源：http://zdb.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qmr.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://fgd.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nxy.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ajw.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsr.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cao.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dec.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bci.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lxu.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gon.yuanzhike.top

================================================================================
来源：http://mfj.chenjidiqi.icu

J. 日期与时间
来源：http://rey.hysaishi.cn

================================================================================
来源：http://gvi.dashuyun.cn

[J01] 获取当前时间
来源：http://oyf.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fvh.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://lpf.xylfe.cn

TS:   new Date();  Date.now()
来源：http://vjd.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yua.hnqzz.top

Go:   time.Now()
来源：http://jkq.ctjpmb.com

Ruby: Time.now
来源：http://njn.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://scn.hongshengwenyu.top

[J02] 格式化输出
来源：http://uld.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eaf.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vcx.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kfs.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://tmg.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fpo.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fuo.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jee.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xrf.xylfe.cn

[J03] 字符串解析为日期
来源：http://nac.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gwa.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fih.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://xgv.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://xgs.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://vux.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dpo.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://rjj.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xjm.jianghu66.top

[J04] 时间戳与日期互转
来源：http://yzr.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://isb.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://peq.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dgs.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lwm.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://odv.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qva.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fgz.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rvq.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://rlq.tarul.cn

Py:   now + timedelta(days=7)
来源：http://eck.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bnl.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkk.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbz.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://wbj.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xbs.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://jfr.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://lom.zycfv.cn

[J06] 计算两时间之差
来源：http://tvj.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://ozk.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://paj.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iaa.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cvm.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tjn.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://ajv.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://jaq.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://yay.cheryme.top

[J07] 比较两个日期
来源：http://vqe.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://yyi.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vtl.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://xpg.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://lwp.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nsv.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbx.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://yjk.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://sdh.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://csh.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yhe.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jpu.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kiy.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ann.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ccr.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bdf.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cet.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tmk.cucudq.cn

[J09] 时区处理
来源：http://omy.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvh.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqg.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rws.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dfd.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ycw.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://huh.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bkv.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dlr.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://tkt.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yac.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hig.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://njn.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fgs.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://agd.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lds.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xmw.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxm.c1oappe.top

================================================================================
来源：http://muv.jlsjyb.cn

K. JSON 与序列化
来源：http://rhe.bbcook.cn

================================================================================
来源：http://nia.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://qwn.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gyv.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mck.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://wpc.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://mdb.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pni.redwolf501.top

Go:   json.Marshal(obj)
来源：http://fep.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xvq.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://poj.cheryme.top

[K02] JSON 字符串转对象
来源：http://fxg.cucudq.cn

Py:   json.loads(s)
来源：http://uht.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zha.sweek.top

JS:   JSON.parse(s)
来源：http://oxg.sxryk.cn

TS:   JSON.parse(s)
来源：http://rud.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbl.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://mmj.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://mox.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vue.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://aqx.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xyk.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mxq.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dbr.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://pje.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lam.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xyb.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://lra.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ixz.cheryme.top

[K04] 读取 JSON 文件
来源：http://ssp.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nmz.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xva.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pov.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rae.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xpp.xuanzx.com


<!-- 参考信息 -->