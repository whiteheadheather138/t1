代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rst.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xch.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://tfw.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fpl.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://bie.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vtw.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://gbk.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xzr.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://oym.bbcook.cn

JS:   Object.entries(obj)
来源：http://uxq.gotoacloud.top

TS:   Object.entries(obj)
来源：http://zhr.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxg.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mop.0kj1m.cn

Ruby: obj.instance_variables
来源：http://vrt.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://hfa.sufxvd.cn

================================================================================
来源：http://xxm.yj20258888.top

H. 异常与错误处理
来源：http://tat.yj202588.top

================================================================================
来源：http://yrb.bbcook.cn

[H01] try / catch 基础
来源：http://lxb.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kzm.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://euu.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ukc.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjd.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ake.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://giy.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cmw.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pbq.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://wuh.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://sse.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xhx.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yaq.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://khq.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rhn.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vqz.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lxo.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cbf.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://eqd.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://zyw.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fpx.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://cyb.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://gso.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://cxm.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bnf.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://btd.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://qzd.sjlbkw.cn

[H04] 自定义异常类型
来源：http://kyg.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://bem.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gjn.316326.xyz

JS:   class MyError extends Error {}
来源：http://ooz.epnwcf.com

TS:   class MyError extends Error {}
来源：http://tcp.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://yrt.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uju.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://yzj.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://sdz.kuanghao11.cn

[H05] 捕获特定类型
来源：http://wvz.aibaodan.cn

Py:   except ValueError as e:
来源：http://bmi.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ham.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://yte.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://tii.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://oll.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fop.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://icx.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://okj.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://knt.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://vrg.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://bwq.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://lze.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://efk.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jbw.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dgp.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://iha.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://ptz.uphjek.com

[H07] 断言
来源：http://ndn.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://jde.epnwcf.com

PHP:  assert($x > 0);
来源：http://iyl.yueranfly.top

JS:   console.assert(x > 0);
来源：http://hga.fehbvm.com

TS:   console.assert(x > 0);
来源：http://zhy.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://bod.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lyc.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://xai.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://sdi.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://tdo.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://tnw.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fks.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://pux.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://cse.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xnt.andypj.xyz

Go:   err.Error()
来源：http://ppu.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://oxg.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://pau.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://tzm.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpi.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uvc.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gqg.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rtl.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eao.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ibx.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ozt.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://moz.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://ogw.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vje.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lmb.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lbe.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eeo.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://czm.yonumen.top

Go:   defer f.Close()
来源：http://jre.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cul.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uko.birdmap.top

================================================================================
来源：http://dyd.tianlin.xyz

I. 正则表达式
来源：http://xdq.tian-w.cn

================================================================================
来源：http://ezj.ydjk.org.cn

[I01] 判断是否匹配
来源：http://fhu.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vjx.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://plq.jianghu66.top

JS:   /\d+/.test(s)
来源：http://vjp.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://qsv.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fei.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://veb.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://ihi.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qnw.ctjpmb.com

[I02] 提取所有匹配
来源：http://ldg.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://oyv.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rhv.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cwd.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://otp.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oaw.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pci.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://jcp.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qri.zycfv.cn

[I03] 提取捕获分组
来源：http://ccm.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zzr.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yrk.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvu.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://beh.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ujx.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qrt.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ssy.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yzi.xylfe.cn

[I04] 正则替换
来源：http://rqv.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fyr.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sos.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dox.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://qpz.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://qcu.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nsp.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fgw.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cvz.fehbvm.com

[I05] 按正则拆分
来源：http://wpd.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://clx.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ebf.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://jbo.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xwd.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://yat.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xze.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://sdy.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kpf.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uut.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eza.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uht.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zkn.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jld.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tws.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgc.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibl.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsy.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://jzn.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://auc.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ryo.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ugz.yonumen.top

TS:   /error/gim
来源：http://xvu.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ncl.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://khh.meibo888.top

Ruby: s.scan(/error/i)
来源：http://ziu.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hfd.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://xjd.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kko.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tju.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://umj.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgo.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nek.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vbq.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hse.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hpk.nanxinkj.top

================================================================================
来源：http://ioh.dashuyun.cn

J. 日期与时间
来源：http://noj.shanyushiyangtech.top

================================================================================
来源：http://lrw.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://ebl.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyf.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsa.shuidangran.top

JS:   new Date();  Date.now()
来源：http://kqs.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://pyq.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://njj.jiagoushi.top

Go:   time.Now()
来源：http://iux.nanxuanxn.top

Ruby: Time.now
来源：http://szn.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aku.fktsv.cn

[J02] 格式化输出
来源：http://uxo.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipi.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fhl.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szq.jlsjyb.cn

TS:   d.toISOString()
来源：http://zpr.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dli.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jos.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wgi.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jbr.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://mqy.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lmj.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rzj.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://ggk.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://qcd.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rxv.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://glm.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://rwd.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbz.vehdjk.com

[J04] 时间戳与日期互转
来源：http://xbz.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pen.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://srw.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mxr.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tvl.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yun.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ken.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://war.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://upx.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://lkq.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://bma.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://inj.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dna.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jpu.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://kyh.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://frp.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://ouc.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://yca.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://vlr.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://cbt.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://rfn.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mvh.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://niq.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ftw.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://ihu.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://ubd.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://qun.nanxinkj.top

[J07] 比较两个日期
来源：http://ivj.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://wtm.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rfh.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://isw.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://svo.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://anb.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lmz.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hdm.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://cbk.yj20258888.top

[J08] 提取年月日与星期
来源：http://cxj.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgn.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nou.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://snf.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://esm.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wdz.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mhs.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bgi.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://znm.havefunace.top

[J09] 时区处理
来源：http://vqt.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vme.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ywj.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxf.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkv.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fep.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://prr.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yso.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wvc.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://rlt.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pww.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ixf.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fkp.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jow.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nly.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iwj.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://srm.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kzu.vehdjk.com

================================================================================
来源：http://nss.hywenlv.cn

K. JSON 与序列化
来源：http://mtl.nanxinkj.top

================================================================================
来源：http://tkw.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://npi.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://omh.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gla.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://vlt.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://kqk.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qvs.xziqi.cn

Go:   json.Marshal(obj)
来源：http://giu.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nhi.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://fum.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://twp.jqgufenzy.top

Py:   json.loads(s)
来源：http://sfm.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://icv.pycfn.com

JS:   JSON.parse(s)
来源：http://npq.aizwys.cn

TS:   JSON.parse(s)
来源：http://bqg.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://caj.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://jqu.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://tuw.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://krq.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://els.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zfz.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://myj.52xcode.cn


<!-- 参考信息 -->