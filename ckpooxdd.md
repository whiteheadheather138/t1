代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://tid.yfazqb.com

Ruby: obj.instance_variables
来源：http://kjy.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://cmj.jyoumei.cn

================================================================================
来源：http://hgs.fengsongda.top

H. 异常与错误处理
来源：http://efr.yonumen.top

================================================================================
来源：http://fei.uphjek.com

[H01] try / catch 基础
来源：http://fgs.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aos.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rhe.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uyt.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjg.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ths.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rlg.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ykf.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rkj.bbcook.cn

[H02] finally / ensure 收尾
来源：http://gop.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://hne.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oue.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jvd.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wty.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://stp.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://amp.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://htd.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dky.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://vyn.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://yac.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzy.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://xvw.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://bot.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zxb.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vwx.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pmm.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://syv.316326.xyz

[H04] 自定义异常类型
来源：http://ypj.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://iwr.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rus.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://kqv.yj20258.top

TS:   class MyError extends Error {}
来源：http://lwi.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://ftm.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cim.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://xfw.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://gyy.cqqwz.cn

[H05] 捕获特定类型
来源：http://uxf.tianlin.xyz

Py:   except ValueError as e:
来源：http://ltu.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbg.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://ouk.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://iyx.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://qfc.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngg.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://mck.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mwg.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://uqe.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://vkn.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://duc.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://pfs.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://nex.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ymy.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fco.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://cvj.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://xxd.chenzaomai.com

[H07] 断言
来源：http://gxl.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://rrb.jinqigufen.top

PHP:  assert($x > 0);
来源：http://cte.andypj.xyz

JS:   console.assert(x > 0);
来源：http://yfr.yongpay.top

TS:   console.assert(x > 0);
来源：http://ehn.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://rmi.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tpb.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://jfa.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://wmv.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://zci.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://fcz.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://adi.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://fhp.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://itz.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xze.ivvv.top

Go:   err.Error()
来源：http://rcn.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://pgq.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://shl.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://ocs.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cnr.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://psh.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://khl.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nke.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drq.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hhz.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rbo.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oke.nwbrower.top

[H10] 资源自动释放
来源：http://vgw.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://agu.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggh.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ndj.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ddm.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://srw.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://vhy.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tdm.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mkw.iojbl.cn

================================================================================
来源：http://exs.gzhubu.top

I. 正则表达式
来源：http://fms.zhongyouzk.top

================================================================================
来源：http://izl.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://ohc.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dil.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://kuv.sysykeji.top

JS:   /\d+/.test(s)
来源：http://bzz.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://laz.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohx.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dvz.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://akc.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zhl.yanxiufei.cn

[I02] 提取所有匹配
来源：http://xur.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://skx.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ioa.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpg.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://qvf.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zfn.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ukt.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://lha.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xzg.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://jma.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ylt.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dik.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vyi.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hxl.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gsc.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xnf.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vqp.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hai.zhixingplan.top

[I04] 正则替换
来源：http://soq.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bsm.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sjw.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://xmv.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://cev.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://mdq.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://djj.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ntn.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mse.ybcxt.top

[I05] 按正则拆分
来源：http://wea.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://qad.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uqr.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://xqd.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://ylq.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://ahr.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xhd.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://edn.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qgj.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rhm.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mkr.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://clr.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rku.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pqi.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hhh.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jfv.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tzf.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eeg.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://cwl.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yya.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zml.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ymn.fengsongda.top

TS:   /error/gim
来源：http://ndn.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uos.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://omm.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://ruj.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uif.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://efv.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tpg.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uhr.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uli.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pnz.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rrc.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jxk.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yrl.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mgn.ivvv.top

================================================================================
来源：http://ybe.dianchejie.cn

J. 日期与时间
来源：http://zrx.c1oappe.top

================================================================================
来源：http://gpz.xylfe.cn

[J01] 获取当前时间
来源：http://fms.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cmf.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pcx.yvedp.cn

JS:   new Date();  Date.now()
来源：http://fqr.daxiang520.top

TS:   new Date();  Date.now()
来源：http://yzf.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ksz.hammf.cn

Go:   time.Now()
来源：http://ujk.bbcook.cn

Ruby: Time.now
来源：http://htf.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pat.jinghuilouyu.cn

[J02] 格式化输出
来源：http://qlw.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oav.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wdr.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tfz.hongshengwenyu.top

TS:   d.toISOString()
来源：http://lqd.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lab.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvz.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fqu.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://twj.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://brr.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kfn.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqx.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://vut.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://jug.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kfh.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nrr.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rhf.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yhk.yueranfly.top

[J04] 时间戳与日期互转
来源：http://kfq.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jrd.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mmu.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hja.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://zju.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wko.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://egd.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mwf.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jch.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ebh.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://lem.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iah.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zyq.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pdn.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://nll.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://isb.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://xsa.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qmq.quarkkingdee.top

[J06] 计算两时间之差
来源：http://irw.birdmap.top

Py:   (end - start).total_seconds()
来源：http://gmu.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://vzo.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hvs.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jkp.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://tiv.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://ypg.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://azk.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://rym.jyoumei.cn

[J07] 比较两个日期
来源：http://rxw.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://gws.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlx.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sto.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://ztk.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dhn.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wxo.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jcm.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://jfs.ppjwa.cn

[J08] 提取年月日与星期
来源：http://blz.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nme.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sdq.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vej.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rms.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qed.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nmu.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://abw.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mzp.andypj.xyz

[J09] 时区处理
来源：http://ftg.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xsc.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylv.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdr.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbn.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://crf.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://keu.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wvr.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qlm.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://gof.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://azj.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cfv.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ntp.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oex.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vrd.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lqz.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zkc.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bqr.zycfv.cn

================================================================================
来源：http://wis.yuxming.cn

K. JSON 与序列化
来源：http://bvb.yangfankeji.com

================================================================================
来源：http://vze.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://snf.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://idh.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aag.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://iuh.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://rzf.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hug.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://lvc.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rki.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://taa.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://mjk.shangyingyoupin.top

Py:   json.loads(s)
来源：http://glx.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://spv.chenzaomai.com

JS:   JSON.parse(s)
来源：http://wsi.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://lvk.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vsw.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://bht.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://knl.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tuo.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://zik.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ktk.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqa.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qft.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://txq.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oic.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gkn.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://rph.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kfc.birdmap.top

[K04] 读取 JSON 文件
来源：http://xcm.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hcj.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bwf.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jvy.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jfe.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ltc.guannengcc.top


<!-- 参考信息 -->