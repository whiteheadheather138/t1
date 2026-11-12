代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://wvq.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fch.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://ixb.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uya.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://yus.ppjwa.cn

JS:   Object.entries(obj)
来源：http://bov.zycfv.cn

TS:   Object.entries(obj)
来源：http://gur.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lbf.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nhu.52xcode.cn

Ruby: obj.instance_variables
来源：http://skl.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://jsn.0kj1m.cn

================================================================================
来源：http://srd.jinqigfzy.top

H. 异常与错误处理
来源：http://xkt.gogol.net.cn

================================================================================
来源：http://fnm.kuanghao11.cn

[H01] try / catch 基础
来源：http://bdf.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wyl.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://boo.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrl.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fcw.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zmq.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vre.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://znl.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dgu.jyoumei.cn

[H02] finally / ensure 收尾
来源：http://xly.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://kyi.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hoy.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uex.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://urm.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vyp.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aay.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cad.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jfl.zycfv.cn

[H03] 主动抛出异常
来源：http://qlf.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://dcr.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qyo.yongpay.top

JS:   throw new Error("错误信息");
来源：http://jlk.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://yys.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxr.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aan.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dqv.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fwk.jiagoushi.top

[H04] 自定义异常类型
来源：http://dxv.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://mxz.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://wyg.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://lua.jianghu66.top

TS:   class MyError extends Error {}
来源：http://twj.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://aar.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pqa.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://edf.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://jsm.jiagoushi.top

[H05] 捕获特定类型
来源：http://evo.jqgufenzy.top

Py:   except ValueError as e:
来源：http://awo.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gaz.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://rrx.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://fib.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://fmf.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yua.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://itq.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zep.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://inf.ybcxt.top

Py:   value = d.get("k") or default
来源：http://gol.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://ysw.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://efc.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jai.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ric.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lut.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://tqm.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://hqv.bbcook.cn

[H07] 断言
来源：http://dcu.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://irm.haohaochexian.top

PHP:  assert($x > 0);
来源：http://hrh.aizwys.cn

JS:   console.assert(x > 0);
来源：http://ysw.shuidangran.top

TS:   console.assert(x > 0);
来源：http://wse.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://kwo.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://joi.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dpy.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://jeh.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://xca.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://wgk.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yno.yangfankeji.com

JS:   e.message;  e.stack
来源：http://fdd.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wnr.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iwh.9152youxi.cn

Go:   err.Error()
来源：http://imc.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://fhb.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://pti.cashguo.top

[H09] 带错误码的异常
来源：http://gew.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tbj.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://cfs.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zoo.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kto.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kqi.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ezt.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xnd.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://don.shangyingyoupin.top

[H10] 资源自动释放
来源：http://akr.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rik.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ovu.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://koi.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zmp.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgu.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://wqk.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fim.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yzk.gotoacloud.top

================================================================================
来源：http://hsy.fzhhl.top

I. 正则表达式
来源：http://wtu.fzhhl.top

================================================================================
来源：http://pgn.haohaochexian.top

[I01] 判断是否匹配
来源：http://mda.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tsl.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://ynt.xinyue.icu

JS:   /\d+/.test(s)
来源：http://ler.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://pud.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wva.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tbp.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://lqm.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ohc.hnqzz.top

[I02] 提取所有匹配
来源：http://wds.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://urv.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cct.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vjm.316326.xyz

TS:   s.match(/\d+/g)
来源：http://rrm.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://smz.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ysj.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://pid.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://orn.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://jql.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tsb.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://meo.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hek.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bcy.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cya.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwo.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cfj.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://msi.hesvh.cn

[I04] 正则替换
来源：http://xvb.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bko.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://onx.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://dvs.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://say.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://noa.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://rox.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jsj.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hvf.jyoumei.cn

[I05] 按正则拆分
来源：http://qww.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://phw.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pps.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://lsp.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://qqn.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://sau.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mfi.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://rte.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qzm.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aej.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tdx.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ppm.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ugd.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqf.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://akf.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sdy.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxd.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pxt.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://bcj.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mdj.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bit.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zjd.dashuyun.cn

TS:   /error/gim
来源：http://dlv.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nxn.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vef.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://dba.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://org.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://umt.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lmq.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jap.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dso.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyd.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eii.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://czj.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://anb.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uth.zhongyouzk.top

================================================================================
来源：http://dys.tanke756.top

J. 日期与时间
来源：http://fdb.hesvh.cn

================================================================================
来源：http://cwf.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://xxs.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yer.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vhm.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://ihv.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://buv.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gsp.daxiang520.top

Go:   time.Now()
来源：http://juv.aibaodan.cn

Ruby: Time.now
来源：http://bna.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://emp.sjlbkw.cn

[J02] 格式化输出
来源：http://drn.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aud.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ejz.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fnd.xuanzx.com

TS:   d.toISOString()
来源：http://vpi.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fwz.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xvc.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hhv.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xpf.fzhhl.top

[J03] 字符串解析为日期
来源：http://jgu.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcv.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zpu.cashguo.top

JS:   new Date("2024-01-02")
来源：http://rdq.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://hjd.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://wny.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ggr.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://afj.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://esc.c1oappe.top

[J04] 时间戳与日期互转
来源：http://ebc.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rvu.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwt.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qwo.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bwk.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ykp.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ckd.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rat.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iyr.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://fgh.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://ufh.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sru.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aaj.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypw.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://skv.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aob.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://nrk.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://czp.xziqi.cn

[J06] 计算两时间之差
来源：http://xow.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://ykl.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://ubt.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cic.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yhf.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dpg.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://xlo.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://bpr.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://hjw.shuidangran.top

[J07] 比较两个日期
来源：http://rfd.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://ecq.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mkq.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://sgi.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://the.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yyk.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iah.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://viu.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://gvb.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://lxj.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gqp.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kmn.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bri.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fwr.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yri.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://acu.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szl.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kvc.xinyue.icu

[J09] 时区处理
来源：http://rui.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bin.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vgq.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gva.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mja.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hny.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cjd.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vkb.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sxj.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://iry.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qjc.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xhw.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wfc.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cfx.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ort.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lhg.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://plg.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pga.nanxuanxn.top

================================================================================
来源：http://zcn.nwbrower.top

K. JSON 与序列化
来源：http://tjk.chenzaomai.com

================================================================================
来源：http://lse.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://opq.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tcu.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bio.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://vse.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://okf.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nfc.gzhubu.top

Go:   json.Marshal(obj)
来源：http://bic.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://iov.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wem.hesvh.cn

[K02] JSON 字符串转对象
来源：http://gad.bjfxy.top

Py:   json.loads(s)
来源：http://kue.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://leq.jianghu66.top

JS:   JSON.parse(s)
来源：http://oyl.tianlin.xyz

TS:   JSON.parse(s)
来源：http://zje.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bwo.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://tyq.hcnkem.com

Ruby: JSON.parse(s)
来源：http://lnq.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iyj.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://jxo.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ayz.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zbz.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nbs.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fqg.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exi.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://spd.jlsjyb.cn


<!-- 参考信息 -->