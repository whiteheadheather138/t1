代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nlk.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zsi.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://tdh.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://azh.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://nzs.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zdk.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://ifv.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sjb.cheryme.top

PHP:  get_object_vars($obj);
来源：http://hps.cqqwz.cn

JS:   Object.entries(obj)
来源：http://els.xziqi.cn

TS:   Object.entries(obj)
来源：http://pbn.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://njh.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xeq.tanke756.top

Ruby: obj.instance_variables
来源：http://ohj.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://etj.yj20258.top

================================================================================
来源：http://qti.jinqigufen.top

H. 异常与错误处理
来源：http://olo.bbcook.cn

================================================================================
来源：http://urw.zhiwuduotai.top

[H01] try / catch 基础
来源：http://vby.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bwd.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://emn.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xcl.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgo.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rlk.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kyk.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zyc.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zex.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://uuk.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://tdy.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xdw.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://lnn.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vkc.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tpf.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xwc.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wof.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ulq.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://wvf.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://qfj.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://csh.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://puq.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://pkl.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://vfi.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ijf.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qcv.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://war.jianghu66.top

[H04] 自定义异常类型
来源：http://zyk.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://pzu.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uqg.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://amt.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://vvx.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://fhi.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://skh.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://wow.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://dzt.tian-w.cn

[H05] 捕获特定类型
来源：http://tej.cheryme.top

Py:   except ValueError as e:
来源：http://usv.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eoz.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://xxo.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://uwd.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://waj.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nza.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://lmn.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://opy.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://sbc.uphjek.com

Py:   value = d.get("k") or default
来源：http://zjk.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://yjb.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://pis.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cvb.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cmi.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://hwe.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://pis.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://dbc.dashuyun.cn

[H07] 断言
来源：http://ooa.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://czy.shuidangran.top

PHP:  assert($x > 0);
来源：http://haf.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://skv.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://ggy.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://dgb.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kut.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://hci.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://epw.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://goi.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ltx.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qzr.jianghu66.top

JS:   e.message;  e.stack
来源：http://zbo.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hfg.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hsy.yanxiufei.cn

Go:   err.Error()
来源：http://zxj.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://qhm.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://ogc.jqgufenzy.top

[H09] 带错误码的异常
来源：http://yju.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://khq.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gra.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xpe.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cfu.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ggg.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hal.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ssx.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bmm.gzhubu.top

[H10] 资源自动释放
来源：http://tsp.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ulg.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sja.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fkc.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hoc.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ieo.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://gzo.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vow.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mkv.kuanghao11.cn

================================================================================
来源：http://thd.c1oappe.top

I. 正则表达式
来源：http://bgh.c1oappe.top

================================================================================
来源：http://drz.aibaodan.cn

[I01] 判断是否匹配
来源：http://mnc.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://whs.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hgb.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://ztx.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://czc.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://myh.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://itz.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://gpk.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://joa.zhengqikj.top

[I02] 提取所有匹配
来源：http://zzv.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://mti.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://auv.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hxj.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://cjj.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ulp.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fze.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://civ.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mzz.uphjek.com

[I03] 提取捕获分组
来源：http://byg.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jhy.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://msy.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sum.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jhs.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://epi.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://end.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://efw.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xzs.jqgfzy.top

[I04] 正则替换
来源：http://unu.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://muu.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cll.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://xfm.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pan.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://tej.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nwy.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rpu.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhd.cucudq.cn

[I05] 按正则拆分
来源：http://toc.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tmt.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kdg.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://bqx.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://zmp.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://dsf.meibo888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xzv.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://son.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nrt.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pxi.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mgl.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vkm.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mjl.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyn.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwr.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vso.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://clf.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rbf.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://nvc.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://too.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kra.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wow.nwbrower.top

TS:   /error/gim
来源：http://gmw.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://duh.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://soy.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://hxq.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ube.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://irk.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ilk.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jfa.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://awa.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xud.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wqo.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sbd.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aeg.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nrz.sysykeji.top

================================================================================
来源：http://qfw.vehdjk.com

J. 日期与时间
来源：http://mpx.sysykeji.top

================================================================================
来源：http://kbm.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://thw.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ffw.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsq.andypj.xyz

JS:   new Date();  Date.now()
来源：http://ndk.316326.xyz

TS:   new Date();  Date.now()
来源：http://rqy.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ucs.xziqi.cn

Go:   time.Now()
来源：http://hru.chenzaomai.com

Ruby: Time.now
来源：http://xxt.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zqg.redwolf501.top

[J02] 格式化输出
来源：http://ocr.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhm.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bhx.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jnp.svipenyu.cn

TS:   d.toISOString()
来源：http://mdx.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://svp.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aao.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://akm.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nti.ybcxt.top

[J03] 字符串解析为日期
来源：http://vzr.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dbg.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xkk.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://lob.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://nyf.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://ewm.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ayr.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://dyo.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nax.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://gjh.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uwp.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://acj.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qlu.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cdc.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kam.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qbt.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sxb.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xcu.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://ciy.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://ijv.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dqj.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iyc.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://msf.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://bhp.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uzw.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://csu.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://umd.zhijiandao.cn

[J06] 计算两时间之差
来源：http://jwu.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://njb.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://dbv.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qau.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oty.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rcd.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://rkt.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://tgt.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://twx.xinyue.icu

[J07] 比较两个日期
来源：http://tfn.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://onb.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uhh.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lgx.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dea.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pao.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xvs.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pnk.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://oat.yuanzhike.top

[J08] 提取年月日与星期
来源：http://kzx.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gjn.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uuc.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vtb.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xih.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://drg.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rfg.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vwc.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gao.ybcxt.top

[J09] 时区处理
来源：http://uxe.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://anz.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yzt.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhd.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kdd.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bah.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lcm.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pun.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nnt.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://bwy.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mss.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwd.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aaj.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://juq.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://slo.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wsb.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gub.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kcs.smart0.xyz

================================================================================
来源：http://obr.sxryk.cn

K. JSON 与序列化
来源：http://hsz.xingfuxueyuan.xyz

================================================================================
来源：http://xgy.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://rck.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qsr.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://obr.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://avw.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://baq.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kra.yuxming.cn

Go:   json.Marshal(obj)
来源：http://nxm.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://aaf.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cyo.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://ajl.guannengcc.top

Py:   json.loads(s)
来源：http://tmx.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ioo.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://fro.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://wdg.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lkw.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ftv.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://jlm.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lid.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://pew.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jai.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://man.nanxinkj.top


<!-- 参考信息 -->