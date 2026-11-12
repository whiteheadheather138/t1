代发 wailian999

PHP:  get_object_vars($obj);
来源：http://pmp.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://hml.yj20258888.top

TS:   Object.entries(obj)
来源：http://mng.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mkb.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://she.hesvh.cn

Ruby: obj.instance_variables
来源：http://kcu.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://riz.jqgfzy.top

================================================================================
来源：http://gso.hammf.cn

H. 异常与错误处理
来源：http://rfo.xziqi.cn

================================================================================
来源：http://rms.hnqzz.top

[H01] try / catch 基础
来源：http://yuq.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kvc.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xiw.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lce.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dym.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yfe.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://enu.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://diz.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dhw.wangdashe.top

[H02] finally / ensure 收尾
来源：http://fww.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://xcu.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://div.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://smu.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nqi.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://scs.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cmu.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://uwy.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ilm.nanxuanxn.top

[H03] 主动抛出异常
来源：http://ldy.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://cbc.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ofg.ivvv.top

JS:   throw new Error("错误信息");
来源：http://qyu.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://dsu.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nsc.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mna.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jhi.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://rpv.yongpay.top

[H04] 自定义异常类型
来源：http://mtx.cashguo.top

Py:   class MyError(Exception): pass
来源：http://qmc.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://wmi.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://obs.smart0.xyz

TS:   class MyError extends Error {}
来源：http://xyg.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://liq.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xap.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://xgo.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://pwo.birdmap.top

[H05] 捕获特定类型
来源：http://rlu.xylfe.cn

Py:   except ValueError as e:
来源：http://mxz.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wtm.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://axv.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://pvj.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://szi.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pak.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://sen.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kkd.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://vyq.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://jia.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lre.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://zzs.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kol.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yyi.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://nkx.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://eqs.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://zld.xylfe.cn

[H07] 断言
来源：http://yle.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://szv.jyoumei.cn

PHP:  assert($x > 0);
来源：http://hlw.nwbrower.top

JS:   console.assert(x > 0);
来源：http://dni.xinyue.icu

TS:   console.assert(x > 0);
来源：http://stt.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://skk.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://trf.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://ivb.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://qls.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://rhf.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://anb.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gap.fktsv.cn

JS:   e.message;  e.stack
来源：http://uou.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uba.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://emd.yuxming.cn

Go:   err.Error()
来源：http://bes.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://gyl.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://kjj.yuanzhike.top

[H09] 带错误码的异常
来源：http://eyg.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jsk.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vlk.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vqt.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xbc.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zst.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dsg.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oev.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jrx.shzxlz.cn

[H10] 资源自动释放
来源：http://zfj.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jft.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ike.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://djj.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qwd.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vnb.wangshuangyany.cn

Go:   defer f.Close()
来源：http://eqw.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mrf.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://inm.zhengqikj.top

================================================================================
来源：http://lgo.zhaomingkeji.xyz

I. 正则表达式
来源：http://usy.zhengqikj.top

================================================================================
来源：http://sug.aizwys.cn

[I01] 判断是否匹配
来源：http://jxu.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kjj.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://etn.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://pwx.daxiang520.top

TS:   /\d+/.test(s)
来源：http://wwj.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hel.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wpd.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://jza.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xyl.haohaochexian.top

[I02] 提取所有匹配
来源：http://ygk.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://pzz.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mmm.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rdr.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://jrc.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fxy.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fuk.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://rgp.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zqx.hnqzz.top

[I03] 提取捕获分组
来源：http://ihz.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pzy.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bqa.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zjv.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ayp.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nan.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chb.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://arm.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://llu.nwbrower.top

[I04] 正则替换
来源：http://gti.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://syj.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ytd.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://elz.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://ubv.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://iod.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://emj.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://emr.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kdm.bbcook.cn

[I05] 按正则拆分
来源：http://pay.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://poo.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dau.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hvz.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://yim.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://mrg.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jfq.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://mga.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nfj.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dqi.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jwu.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtn.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aqj.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nuy.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vfy.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://are.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://soi.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://euo.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://oow.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uot.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xpr.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://anr.cheryme.top

TS:   /error/gim
来源：http://pmv.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://khl.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://grv.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://wno.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://spu.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://vxe.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vii.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zuh.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igj.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://raa.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kil.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jav.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hfh.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://knx.smart0.xyz

================================================================================
来源：http://qlr.fzhhl.top

J. 日期与时间
来源：http://bdp.cqqwz.cn

================================================================================
来源：http://vab.andypj.xyz

[J01] 获取当前时间
来源：http://dbq.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cys.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aeu.yongpay.top

JS:   new Date();  Date.now()
来源：http://iqx.aizwys.cn

TS:   new Date();  Date.now()
来源：http://jrc.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ifc.zycfv.cn

Go:   time.Now()
来源：http://bri.jyoumei.cn

Ruby: Time.now
来源：http://pto.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://svm.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://omd.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cej.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sbk.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yqk.tarul.cn

TS:   d.toISOString()
来源：http://fln.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ohi.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dsi.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aed.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zio.chenzaomai.com

[J03] 字符串解析为日期
来源：http://xbu.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iss.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iho.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://qsb.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://ome.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://urt.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qvi.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://sfg.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zrt.yueranfly.top

[J04] 时间戳与日期互转
来源：http://esc.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ors.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sbb.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://taa.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tae.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dqj.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pmq.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://upj.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hux.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://uuu.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://nof.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rjp.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mhu.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpf.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://ick.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwo.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://zsg.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://lsd.yj20258.top

[J06] 计算两时间之差
来源：http://bgl.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://uik.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://kdp.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gtc.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iaw.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fam.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://wgs.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://mxt.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://xca.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://iuc.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://vmg.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lpc.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://xhi.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://exb.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://foy.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bie.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://khd.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://mlh.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://brr.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pkj.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cpw.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://muj.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://szb.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkv.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://srq.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agk.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uok.xinyue.icu

[J09] 时区处理
来源：http://nnh.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fix.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ngc.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlk.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwc.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rpx.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fns.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://aog.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gjz.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://cyl.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zdo.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qhz.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rdg.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjf.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gtb.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sam.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wxb.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vwn.hammf.cn

================================================================================
来源：http://fzo.jiagoushi.top

K. JSON 与序列化
来源：http://tfm.cheryme.top

================================================================================
来源：http://ehg.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://ija.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hmh.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sim.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://qbf.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://ooa.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dcu.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://rnx.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://dfz.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eqt.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://auf.xuanzx.com

Py:   json.loads(s)
来源：http://xpb.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pfs.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://qxa.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://pgr.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://edm.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://cin.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://zge.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ntf.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://iaj.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://luj.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yfu.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cnd.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lut.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqq.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rbl.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://srw.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wuu.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://kbz.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://voq.yj202588.top


<!-- 参考信息 -->