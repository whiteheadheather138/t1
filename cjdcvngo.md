代发 wailian999

PHP:  get_object_vars($obj);
来源：http://zfw.gotoacloud.top

JS:   Object.entries(obj)
来源：http://sip.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://pzk.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qqx.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ncy.tianlin.xyz

Ruby: obj.instance_variables
来源：http://cmn.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://loa.chenzaomai.com

================================================================================
来源：http://xiq.sxryk.cn

H. 异常与错误处理
来源：http://ser.pycfn.com

================================================================================
来源：http://upi.vqdsnc.cn

[H01] try / catch 基础
来源：http://jyl.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zih.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jsl.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://edg.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hya.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gta.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rho.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fdg.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fju.xuanzx.com

[H02] finally / ensure 收尾
来源：http://lpj.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pxs.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fxf.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sjh.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ppn.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kgb.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kqb.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://cse.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://frg.hesvh.cn

[H03] 主动抛出异常
来源：http://yvc.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://txj.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://idy.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://xbm.yongpay.top

TS:   throw new Error("错误信息");
来源：http://bax.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xhe.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://emm.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vhj.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://iam.hnqzz.top

[H04] 自定义异常类型
来源：http://rbs.meibo888.top

Py:   class MyError(Exception): pass
来源：http://zed.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://eyr.bbcook.cn

JS:   class MyError extends Error {}
来源：http://gls.hnqzz.top

TS:   class MyError extends Error {}
来源：http://pev.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://xig.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wes.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://ecx.hammf.cn

C#:   class MyException : Exception {}
来源：http://vhn.xinyue.icu

[H05] 捕获特定类型
来源：http://oyp.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://znl.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mjg.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://hdt.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://dyz.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://xru.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xmk.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://zza.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://smr.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://zud.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://isi.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://gvr.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://yal.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://tbm.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwp.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mdh.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://sfk.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://qeu.hcnkem.com

[H07] 断言
来源：http://sxi.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://enj.daria6918.cn

PHP:  assert($x > 0);
来源：http://ehl.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://qim.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://ohm.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://iis.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fyz.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://nxl.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://xfu.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://dnk.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://bgu.zdqjudy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbx.tarul.cn

JS:   e.message;  e.stack
来源：http://vbz.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qyw.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eea.zhaomingkeji.xyz

Go:   err.Error()
来源：http://vss.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://hwj.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://vpn.meibo888.top

[H09] 带错误码的异常
来源：http://lal.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ync.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lhy.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zgf.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fkd.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ert.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fye.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mxj.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gol.yueranfly.top

[H10] 资源自动释放
来源：http://qms.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkj.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mci.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vge.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fht.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ooi.jlsjyb.cn

Go:   defer f.Close()
来源：http://akh.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjj.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxs.cashguo.top

================================================================================
来源：http://rzp.zhiwuduotai.top

I. 正则表达式
来源：http://ysn.52xcode.cn

================================================================================
来源：http://kpg.meibo888.top

[I01] 判断是否匹配
来源：http://bnj.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gvi.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fef.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://tyi.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://pwz.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qty.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tiq.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://tsm.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cah.hysaishi.cn

[I02] 提取所有匹配
来源：http://tub.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://dnm.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lae.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyj.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://gxt.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkq.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bjm.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://ypc.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qay.andypj.xyz

[I03] 提取捕获分组
来源：http://ipa.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ixl.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yus.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qnc.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rqr.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kes.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qtu.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gmd.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rxa.hnqzz.top

[I04] 正则替换
来源：http://wcf.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://czm.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iws.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://uue.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hee.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://mlc.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://omn.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pjx.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pbz.cashguo.top

[I05] 按正则拆分
来源：http://gsu.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zhf.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vqh.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://nui.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://glj.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://qdj.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://csc.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://qci.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bto.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kqp.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mwc.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://msb.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://moz.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kpc.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://khz.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vnw.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oha.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gmy.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://mcm.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kvw.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ywj.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://adp.gotoacloud.top

TS:   /error/gim
来源：http://lhx.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uup.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ndk.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://xag.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cbh.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://qkq.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oqb.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nrz.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nhg.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nie.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jkb.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cdr.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dhc.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lut.jinyuanbaomall.cn

================================================================================
来源：http://tgz.birdmap.top

J. 日期与时间
来源：http://seq.hywenlv.cn

================================================================================
来源：http://zfw.dianchejie.cn

[J01] 获取当前时间
来源：http://qtq.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oal.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wyy.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://urg.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://epa.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mqp.quarkkingdee.top

Go:   time.Now()
来源：http://jkb.tarul.cn

Ruby: Time.now
来源：http://tod.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qln.jinqigfzy.top

[J02] 格式化输出
来源：http://qzc.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wnm.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yqf.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fjz.xylfe.cn

TS:   d.toISOString()
来源：http://vdp.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ytk.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udo.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zfr.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pzq.xuanzx.com

[J03] 字符串解析为日期
来源：http://rkp.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yxu.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://esp.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://hfz.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://tic.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://xif.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zak.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://jqm.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxt.nwbrower.top

[J04] 时间戳与日期互转
来源：http://fva.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://haw.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://duh.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://djs.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://xir.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tph.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kkh.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pen.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wws.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://yoq.tanke756.top

Py:   now + timedelta(days=7)
来源：http://mhb.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gvq.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hws.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://det.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://lew.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ihs.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://nzk.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zxa.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://uin.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://srz.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://coz.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uvt.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://syl.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://pyt.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://vso.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://vol.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://qdn.smart0.xyz

[J07] 比较两个日期
来源：http://gnk.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://qeb.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ioh.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://dxv.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://myd.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atq.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ywr.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://msk.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zfq.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://pyb.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oyz.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tmd.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bjo.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ecv.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hls.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rvw.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tmr.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lkk.yj202588.top

[J09] 时区处理
来源：http://opj.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bit.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dbz.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dhi.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qph.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vri.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ehk.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://pke.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fyz.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://flp.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jcf.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vjp.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gpu.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pfe.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fep.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wss.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://klv.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yfg.tanke756.top

================================================================================
来源：http://vdy.smart0.xyz

K. JSON 与序列化
来源：http://mkl.birdmap.top

================================================================================
来源：http://gyk.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://cpa.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qva.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://isp.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://kdm.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://nkm.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mfw.mhx1999.top

Go:   json.Marshal(obj)
来源：http://rog.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zsj.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mvf.52xcode.cn

[K02] JSON 字符串转对象
来源：http://nvd.zhoulong.xyz

Py:   json.loads(s)
来源：http://opm.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://grj.smart0.xyz

JS:   JSON.parse(s)
来源：http://efk.zdqjudy.top

TS:   JSON.parse(s)
来源：http://zvm.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bwf.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ydd.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://hhw.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://url.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://npc.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gsp.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://krf.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://bki.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jwa.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hhz.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lwi.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://num.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyu.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://qpr.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ymc.xylfe.cn


<!-- 参考信息 -->