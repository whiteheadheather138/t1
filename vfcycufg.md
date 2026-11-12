代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://aoq.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xjl.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://qrd.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xpo.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://tkm.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://xvm.fzhhl.top

TS:   Object.entries(obj)
来源：http://ujr.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cqw.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://mpj.meibo888.top

Ruby: obj.instance_variables
来源：http://jkm.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ahe.redwolf501.top

================================================================================
来源：http://thm.ybcxt.top

H. 异常与错误处理
来源：http://owx.9152youxi.cn

================================================================================
来源：http://uqv.shuidangran.top

[H01] try / catch 基础
来源：http://kpk.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dzc.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ytl.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uon.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://piq.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kyq.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fju.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kdx.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nsn.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://zrg.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hul.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gry.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://raz.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://nsw.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://jrk.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ssw.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rxy.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ugz.yanxiufei.cn

[H03] 主动抛出异常
来源：http://ske.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://jce.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jex.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://dhf.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://bnu.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vgw.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sby.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sax.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://fxp.sufxvd.cn

[H04] 自定义异常类型
来源：http://dfs.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://gai.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://zfa.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://auw.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://atw.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://bqr.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mtc.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://wag.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://acu.tarul.cn

[H05] 捕获特定类型
来源：http://btb.meibo888.top

Py:   except ValueError as e:
来源：http://urb.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cjk.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://snl.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://qjz.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://dcq.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kxx.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://zbt.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://utg.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://ewq.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://yix.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hdx.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://ehm.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dty.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pkf.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nra.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://aht.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://xbt.pengpengdd.cyou

[H07] 断言
来源：http://mmg.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://pfs.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://hln.xziqi.cn

JS:   console.assert(x > 0);
来源：http://vuq.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://ufr.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://lje.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qyq.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://qtu.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://vbo.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://fir.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://efq.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ntk.52xcode.cn

JS:   e.message;  e.stack
来源：http://erw.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bou.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://laq.vehdjk.com

Go:   err.Error()
来源：http://bug.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://qez.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://mne.xinyue.icu

[H09] 带错误码的异常
来源：http://ios.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://slt.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tps.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vvc.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ygc.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mhg.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://olj.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ktw.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://guf.jianghu66.top

[H10] 资源自动释放
来源：http://crn.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ode.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bij.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dsi.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://owr.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mud.sjlbkw.cn

Go:   defer f.Close()
来源：http://jsx.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wuk.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jbk.cqqwz.cn

================================================================================
来源：http://xpf.shzxlz.cn

I. 正则表达式
来源：http://xgl.zhongyouzk.top

================================================================================
来源：http://pzm.tian-w.cn

[I01] 判断是否匹配
来源：http://qwh.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iac.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vyp.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://cps.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://mhk.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://izo.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oiy.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://xxh.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yqt.sxryk.cn

[I02] 提取所有匹配
来源：http://bfd.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://fpd.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wsh.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dud.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://dnb.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xab.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ioc.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://wsx.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sld.jqgfzy.top

[I03] 提取捕获分组
来源：http://yux.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aco.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asn.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://plq.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ggz.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bry.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nok.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hpb.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nrm.gaohongyu789.top

[I04] 正则替换
来源：http://plr.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lhy.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pym.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://wum.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jhf.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hmk.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oxo.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jmq.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gvl.zycfv.cn

[I05] 按正则拆分
来源：http://rhf.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pcp.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvq.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://oxv.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://vmk.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://nvb.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ijc.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://fes.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uwu.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://epu.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fve.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtg.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kiy.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lta.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fyc.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gvj.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ezd.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nus.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://awr.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://thh.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tyv.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pev.shanyushiyangkeji.top

TS:   /error/gim
来源：http://fhu.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yld.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wlj.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://sgs.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cqm.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://jfo.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zgf.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xsc.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://url.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfz.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dwm.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://whu.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvi.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lpo.hcnkem.com

================================================================================
来源：http://ilf.aizwys.cn

J. 日期与时间
来源：http://rpc.shanyushiyangkeji.top

================================================================================
来源：http://see.shuidangran.top

[J01] 获取当前时间
来源：http://mfu.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qmz.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://egk.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://egw.xuanzx.com

TS:   new Date();  Date.now()
来源：http://dcu.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nkr.yuanzhike.top

Go:   time.Now()
来源：http://tfu.shangyingyoupin.top

Ruby: Time.now
来源：http://mup.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qga.jyoumei.cn

[J02] 格式化输出
来源：http://jcj.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aie.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iyt.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ajc.yueranfly.top

TS:   d.toISOString()
来源：http://ywz.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://myw.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jfo.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://arm.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xwt.yangfankeji.com

[J03] 字符串解析为日期
来源：http://mbm.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://izx.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ovd.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://snb.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://mxl.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://xkx.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ygu.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://ibn.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tnk.c1oappe.top

[J04] 时间戳与日期互转
来源：http://jpw.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jyd.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ehm.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ecr.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://afg.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://urz.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cxs.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpo.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://itd.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://beh.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://kqq.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pua.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ghc.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpl.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://dxn.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cam.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://ivr.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://cvl.smart0.xyz

[J06] 计算两时间之差
来源：http://fji.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://vlo.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://etr.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kyf.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cdh.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ypg.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://oqk.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://dmd.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://jfs.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://ohj.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://qkx.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oho.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://hcw.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://gjq.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kun.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nzx.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://gae.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://prb.hywenlv.cn

[J08] 提取年月日与星期
来源：http://mbv.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brb.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ehn.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rko.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pqu.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iah.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qnz.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tnq.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulw.hnqzz.top

[J09] 时区处理
来源：http://dyn.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfa.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kmy.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yna.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://foh.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vvw.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://flg.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://mrl.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lwk.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://nzb.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yln.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://huo.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ivw.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://orj.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hyw.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zpr.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gyo.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mbf.jlsjyb.cn

================================================================================
来源：http://kmm.quarkkingdee.top

K. JSON 与序列化
来源：http://dkj.yangfankeji.com

================================================================================
来源：http://jiu.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://hem.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ijj.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zkh.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://imj.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://old.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ccw.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://ddz.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bsp.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://swe.shuidangran.top

[K02] JSON 字符串转对象
来源：http://xld.smart0.xyz

Py:   json.loads(s)
来源：http://fwv.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pru.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://jea.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://gpk.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xle.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://xjs.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://wfk.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hio.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://vld.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hkd.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nag.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xak.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ybp.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tgo.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikk.yfazqb.com


<!-- 参考信息 -->