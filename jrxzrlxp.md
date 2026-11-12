代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fim.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cfc.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://mub.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ath.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://ofz.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://upr.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://jdg.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cry.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://yei.hywenlv.cn

JS:   Object.entries(obj)
来源：http://for.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ayy.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://whf.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://thh.hysaishi.cn

Ruby: obj.instance_variables
来源：http://jll.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://zuh.tanke756.top

================================================================================
来源：http://dxy.xinyue.icu

H. 异常与错误处理
来源：http://jie.jinyuanbaomall.cn

================================================================================
来源：http://luq.jinqigfzy.top

[H01] try / catch 基础
来源：http://zzz.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxs.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vvg.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpg.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tqd.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ikq.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjh.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wok.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wxk.xylfe.cn

[H02] finally / ensure 收尾
来源：http://bkd.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dvs.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zyo.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hnb.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qtf.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://vlb.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rhw.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yjr.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lks.jiagoushi.top

[H03] 主动抛出异常
来源：http://jnb.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://qyh.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hya.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://jvt.316326.xyz

TS:   throw new Error("错误信息");
来源：http://pra.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ewc.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aho.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ywl.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://paq.xziqi.cn

[H04] 自定义异常类型
来源：http://otj.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://bzl.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://tof.cashguo.top

JS:   class MyError extends Error {}
来源：http://yxj.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://oup.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://lqc.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qxe.sweek.top

Ruby: class MyError < StandardError; end
来源：http://cws.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://snm.ppjwa.cn

[H05] 捕获特定类型
来源：http://xfb.tianlin.xyz

Py:   except ValueError as e:
来源：http://tyz.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fkt.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://hul.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://rwd.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://mld.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://puq.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://dwz.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://apj.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://uqd.aizwys.cn

Py:   value = d.get("k") or default
来源：http://awx.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dgm.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://xko.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://dpt.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dgf.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qcb.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://zbw.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://aec.chenzaomai.com

[H07] 断言
来源：http://ydr.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://yid.yj20258888.top

PHP:  assert($x > 0);
来源：http://wdv.epnwcf.com

JS:   console.assert(x > 0);
来源：http://mkp.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://ngn.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://xwe.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bhe.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://qvu.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://cfl.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://von.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://qck.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zhy.hysaishi.cn

JS:   e.message;  e.stack
来源：http://arr.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://drn.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ftx.shangyingyoupin.top

Go:   err.Error()
来源：http://msh.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://uhy.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://blt.chenzaomai.com

[H09] 带错误码的异常
来源：http://iwv.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://umj.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jpy.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zag.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lgf.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dks.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hia.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zgr.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nkh.jinqigufen.top

[H10] 资源自动释放
来源：http://zum.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ouf.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hjd.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://deu.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tdv.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://unt.hysaishi.cn

Go:   defer f.Close()
来源：http://das.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://irr.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yck.zdbjq.cn

================================================================================
来源：http://eqh.xuetiantiany.cn

I. 正则表达式
来源：http://scn.mhx1999.top

================================================================================
来源：http://xzq.birdmap.top

[I01] 判断是否匹配
来源：http://tps.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbp.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ohx.sweek.top

JS:   /\d+/.test(s)
来源：http://uwi.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://num.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aza.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vyp.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://ynz.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mot.svipenyu.cn

[I02] 提取所有匹配
来源：http://iff.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://kut.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xzc.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpg.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://qvu.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bjq.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tot.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://qpf.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csg.kuanghao11.cn

[I03] 提取捕获分组
来源：http://nph.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ykj.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://flx.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pbl.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kjg.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bwt.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jpl.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pks.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lxi.jiagoushi.top

[I04] 正则替换
来源：http://yvj.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gnm.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hiq.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://erg.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://nwn.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://vya.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://opz.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ijw.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tpz.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://zri.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tnp.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vie.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://ylq.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://ipw.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://afh.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mhq.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rgs.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vzh.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mmt.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ndd.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zge.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iyx.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqb.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ybi.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kho.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rvt.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nuv.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://wll.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kdo.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wkp.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zwf.tanke756.top

TS:   /error/gim
来源：http://eok.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hvm.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zly.uphjek.com

Ruby: s.scan(/error/i)
来源：http://izp.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ali.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://cko.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yev.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nvs.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uto.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uev.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nzq.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hag.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fza.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nul.sysykeji.top

================================================================================
来源：http://hln.ywan-chungtsiang.top

J. 日期与时间
来源：http://vux.hammf.cn

================================================================================
来源：http://vly.havefunace.top

[J01] 获取当前时间
来源：http://ayt.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uln.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bhl.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://xlp.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://stl.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hmq.0kj1m.cn

Go:   time.Now()
来源：http://lsq.sjlbkw.cn

Ruby: Time.now
来源：http://wsc.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jwj.svipenyu.cn

[J02] 格式化输出
来源：http://uil.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://buf.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://prz.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qfs.zycfv.cn

TS:   d.toISOString()
来源：http://ccn.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://per.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zxu.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nhq.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iea.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://tls.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nst.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zef.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://lnm.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://pfo.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://vob.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://irc.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://uwn.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nmg.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://rla.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ipu.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cqk.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://crc.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://unb.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://plk.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ygd.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bzd.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rzn.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://iiy.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://eqq.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ubk.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dck.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wjh.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://khu.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eja.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://icr.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vsl.jiagoushi.top

[J06] 计算两时间之差
来源：http://rlc.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://pwr.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://agx.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://isl.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bhu.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://lhg.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://jhe.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://ojs.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://sgf.snrcjt.cn

[J07] 比较两个日期
来源：http://zfc.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://oau.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tak.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://xue.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tle.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gbx.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bhf.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://euy.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://ivn.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://flx.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lvq.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ijg.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gwd.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iwg.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sgp.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://urn.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yak.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jbn.fanxiaobao.xyz

[J09] 时区处理
来源：http://huj.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://btp.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nfz.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rsn.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zpy.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://woi.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gac.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mye.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mnk.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://aod.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wmh.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pry.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://shg.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cog.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gbg.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iuc.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzv.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pts.tianlin.xyz

================================================================================
来源：http://bzc.hnqzz.top

K. JSON 与序列化
来源：http://ifm.ywan-chungtsiang.top

================================================================================
来源：http://boz.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://ass.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nkn.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://std.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://bmc.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://nfg.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sbk.xziqi.cn

Go:   json.Marshal(obj)
来源：http://amp.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://tjv.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yyr.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://psf.dianchejie.cn

Py:   json.loads(s)
来源：http://vle.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vwn.fengsongda.top

JS:   JSON.parse(s)
来源：http://qvs.sxryk.cn

TS:   JSON.parse(s)
来源：http://dro.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gmc.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://awz.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://nog.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://umd.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://olg.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rci.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://abq.tarul.cn


<!-- 参考信息 -->