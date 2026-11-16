代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://oyf.birdmap.top

Ruby: obj.instance_variables
来源：http://usk.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://vpo.zdbjq.cn

================================================================================
来源：http://thh.cqqwz.cn

H. 异常与错误处理
来源：http://xhw.sysykeji.top

================================================================================
来源：http://xqz.iojbl.cn

[H01] try / catch 基础
来源：http://pzy.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hsz.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hpi.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ows.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iiy.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lut.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yhs.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://reh.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gop.bjfxy.top

[H02] finally / ensure 收尾
来源：http://nhl.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://brj.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://voy.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ktb.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ifm.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://bma.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nwz.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kwl.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://agz.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://two.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://cuc.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kop.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://mqw.cheryme.top

TS:   throw new Error("错误信息");
来源：http://waq.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ysh.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nwu.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pnb.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qtj.9152youxi.cn

[H04] 自定义异常类型
来源：http://sgk.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://uhj.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ysf.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://hzm.yuxming.cn

TS:   class MyError extends Error {}
来源：http://uvf.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://gge.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://riz.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://yww.hammf.cn

C#:   class MyException : Exception {}
来源：http://aly.hammf.cn

[H05] 捕获特定类型
来源：http://zco.dashuyun.cn

Py:   except ValueError as e:
来源：http://zqn.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ddz.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://lqk.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://mjo.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://kji.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fhj.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://plq.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vfy.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://kdx.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://cwl.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xnk.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://brr.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://tpz.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://flp.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://btk.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://xmr.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://vqb.dashuyun.cn

[H07] 断言
来源：http://eec.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://lda.dashuyun.cn

PHP:  assert($x > 0);
来源：http://myb.mhx1999.top

JS:   console.assert(x > 0);
来源：http://uwc.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://viv.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://ecj.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfn.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bba.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://taz.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://jxv.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://bjd.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zbs.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://sjm.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tql.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kuw.sxryk.cn

Go:   err.Error()
来源：http://kyb.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://tad.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://dpc.yj20258888.top

[H09] 带错误码的异常
来源：http://kpq.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mwu.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://irj.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kdk.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://foy.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hhc.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wea.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dls.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ovz.dashuyun.cn

[H10] 资源自动释放
来源：http://ekf.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xtt.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://chl.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nlc.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ofh.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jxq.cdnleiting.top

Go:   defer f.Close()
来源：http://mjg.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mld.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mgq.fktsv.cn

================================================================================
来源：http://leg.jiagoushi.top

I. 正则表达式
来源：http://hfc.yj202588.top

================================================================================
来源：http://eup.yonumen.top

[I01] 判断是否匹配
来源：http://pnp.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eqj.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qng.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://tjt.yfazqb.com

TS:   /\d+/.test(s)
来源：http://ydc.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ryp.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kfs.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://rmh.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://new.52xcode.cn

[I02] 提取所有匹配
来源：http://adu.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://srj.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jit.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gqo.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://ohy.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bxa.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxu.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://tqv.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rrr.tianlin.xyz

[I03] 提取捕获分组
来源：http://mlz.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lev.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tgg.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ccg.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zfu.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rgd.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kpn.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jqv.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cfd.yj202588.top

[I04] 正则替换
来源：http://osz.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cbd.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ngc.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://atf.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://gvm.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gvz.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://bmb.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lfi.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dzb.zycfv.cn

[I05] 按正则拆分
来源：http://mhw.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wnh.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cou.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://ese.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://fmm.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://riz.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hhr.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://xtc.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xfg.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bpy.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://acf.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nbx.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hrl.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gkk.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pae.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mei.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://syy.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vtj.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://vtf.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eoi.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ekt.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hoc.yuxming.cn

TS:   /error/gim
来源：http://mwp.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kwe.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ypi.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://xgg.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sdq.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://uxo.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dsu.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ccs.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpw.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://efy.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ccs.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wzk.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qhx.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mpe.sxryk.cn

================================================================================
来源：http://cfx.jianghu66.top

J. 日期与时间
来源：http://qee.shuidangran.top

================================================================================
来源：http://ijp.aizwys.cn

[J01] 获取当前时间
来源：http://bwc.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qzk.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vpt.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://mpu.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://ltg.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aia.zdbjq.cn

Go:   time.Now()
来源：http://krm.xuetiantiany.cn

Ruby: Time.now
来源：http://ewh.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tbl.zhijiandao.cn

[J02] 格式化输出
来源：http://szw.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eom.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://igc.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://equ.cashguo.top

TS:   d.toISOString()
来源：http://fmg.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qle.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zds.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhx.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mis.zhixingplan.top

[J03] 字符串解析为日期
来源：http://qls.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cmp.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mmy.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://dgc.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://sfr.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aws.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oxm.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xki.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xug.xuanzx.com

[J04] 时间戳与日期互转
来源：http://bvx.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tsd.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://afl.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bje.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vby.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ptx.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yii.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bpa.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cvd.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://okc.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://bcx.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmg.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqx.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vic.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://vzn.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxv.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://keg.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://wwn.epnwcf.com

[J06] 计算两时间之差
来源：http://jxd.yongpay.top

Py:   (end - start).total_seconds()
来源：http://vns.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://pbt.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ejr.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hxb.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://htb.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://ywr.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://fjv.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://efy.havefunace.top

[J07] 比较两个日期
来源：http://qum.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://eiu.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zoz.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://llv.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://upe.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pyd.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nvd.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ghq.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://spr.dianchejie.cn

[J08] 提取年月日与星期
来源：http://pmy.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qez.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tie.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vif.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpt.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xzr.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pjj.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lvd.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vqi.yueranfly.top

[J09] 时区处理
来源：http://zvc.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hyg.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lfo.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqe.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbh.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gmv.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wtk.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gho.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gkf.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://lpn.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uda.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jxr.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xlp.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ckv.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwm.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nun.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nab.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iwj.chenjidiqi.icu

================================================================================
来源：http://spj.nanxinkj.top

K. JSON 与序列化
来源：http://azh.yuanzhike.top

================================================================================
来源：http://kjf.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://wwq.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://akn.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ggu.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://dyr.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://ewp.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rmg.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://hdq.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://nsa.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ufu.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://ejz.zhoulong.xyz

Py:   json.loads(s)
来源：http://sui.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bgo.yonumen.top

JS:   JSON.parse(s)
来源：http://ahk.sweek.top

TS:   JSON.parse(s)
来源：http://rvj.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zeq.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://dsz.gzhubu.top

Ruby: JSON.parse(s)
来源：http://hap.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qez.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://vpm.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vka.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zwe.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hyz.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pvk.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kct.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rpp.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yqc.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cks.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://ufv.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://msu.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://itm.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hwi.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpw.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zwj.yj202588.top


<!-- 参考信息 -->