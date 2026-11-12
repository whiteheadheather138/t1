代发 wailian999

C#:   record User(string Name, int Age);
来源：http://yml.svipenyu.cn

[G15] 枚举
来源：http://vdr.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrk.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kcu.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cxb.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yzq.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://yjb.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbn.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://tii.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yji.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://ehy.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sbh.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://rze.chenzaomai.com

JS:   Object.entries(obj)
来源：http://xel.xinyue.icu

TS:   Object.entries(obj)
来源：http://tsq.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtp.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hfs.birdmap.top

Ruby: obj.instance_variables
来源：http://dlc.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://hvf.feifeiyinyue.top

================================================================================
来源：http://aua.fktsv.cn

H. 异常与错误处理
来源：http://tom.jinyuanbaomall.cn

================================================================================
来源：http://ptm.ppjwa.cn

[H01] try / catch 基础
来源：http://tsd.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://obf.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ppn.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fka.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pxx.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwy.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ajq.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xzc.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dps.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://cfk.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hzp.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aze.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oql.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jjn.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://nkb.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://rgy.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pmr.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dvh.yj20258.top

[H03] 主动抛出异常
来源：http://gft.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://xwy.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yqe.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://bmb.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://jgu.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iun.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ntf.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hjy.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://glp.nanxinkj.top

[H04] 自定义异常类型
来源：http://ivt.tarul.cn

Py:   class MyError(Exception): pass
来源：http://euq.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://hvm.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://aym.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://mwj.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://mll.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qiw.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://vka.nwbrower.top

C#:   class MyException : Exception {}
来源：http://kpt.sysykeji.top

[H05] 捕获特定类型
来源：http://tfi.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://zes.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xxk.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://jal.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://cjq.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://din.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yai.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://iwo.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nwd.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://fah.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://ann.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://jlw.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bol.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://uuf.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://swu.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tou.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://pvp.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://gcu.yanxiufei.cn

[H07] 断言
来源：http://twq.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://mmh.tianlin.xyz

PHP:  assert($x > 0);
来源：http://xru.xylfe.cn

JS:   console.assert(x > 0);
来源：http://btt.cucudq.cn

TS:   console.assert(x > 0);
来源：http://ssp.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://zsm.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jku.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://gbk.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://mop.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://ybe.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://smj.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vtq.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://meu.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://geb.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lqn.hammf.cn

Go:   err.Error()
来源：http://edt.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://hze.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://lbj.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://hii.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rjs.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hkl.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xmh.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bpd.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://afb.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gia.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://rnq.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dct.iojbl.cn

[H10] 资源自动释放
来源：http://efo.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://xkm.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hth.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://flc.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xcb.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://grz.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://tws.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ahj.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wrw.xuetiantiany.cn

================================================================================
来源：http://wtu.jianghu66.top

I. 正则表达式
来源：http://zkb.aizwys.cn

================================================================================
来源：http://ckd.fktsv.cn

[I01] 判断是否匹配
来源：http://vbx.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uak.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://hhj.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://ffz.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://whb.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bkv.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dgj.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://hfa.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pbe.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://ozy.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://qew.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zkf.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pkd.yonumen.top

TS:   s.match(/\d+/g)
来源：http://juo.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dxe.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hlg.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://kcq.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dco.gogol.net.cn

[I03] 提取捕获分组
来源：http://utn.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gqt.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zqi.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bwv.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fur.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pzo.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kdj.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://udj.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://odn.shangyingyoupin.top

[I04] 正则替换
来源：http://tzf.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eli.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffd.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://ewv.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gdd.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://ylq.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mee.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yxl.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://shw.hnqzz.top

[I05] 按正则拆分
来源：http://gbm.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cmx.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vzd.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://cyf.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://vbt.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://hmp.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ved.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gdh.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yfn.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yvq.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tjg.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lqr.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsd.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bad.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ape.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wgb.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rip.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aka.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://dza.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lyr.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pyz.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qjc.jqgufenzy.top

TS:   /error/gim
来源：http://zyw.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://umc.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zot.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://gnk.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lgt.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://hyl.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejy.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mxv.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kdx.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hhs.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://azb.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fml.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://enw.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://quv.mhx1999.top

================================================================================
来源：http://cqb.wangdashe.top

J. 日期与时间
来源：http://anj.52xcode.cn

================================================================================
来源：http://fdz.ybcxt.top

[J01] 获取当前时间
来源：http://mrn.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gfc.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dqm.cashguo.top

JS:   new Date();  Date.now()
来源：http://yul.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://vyb.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rhl.shanyushiyangtech.top

Go:   time.Now()
来源：http://piz.epnwcf.com

Ruby: Time.now
来源：http://lxj.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yel.0kj1m.cn

[J02] 格式化输出
来源：http://xjw.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqe.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ezo.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pua.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://kck.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ako.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bzo.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upx.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tqa.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://dmd.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ijq.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpv.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://err.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://gfq.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://jad.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://joe.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://zxa.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yuq.sxryk.cn

[J04] 时间戳与日期互转
来源：http://ovc.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nlh.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vuh.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wvw.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ilx.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nlt.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sox.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvs.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ruh.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://ihz.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://dfy.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezt.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xal.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://myi.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://qaz.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nku.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://lyu.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://zgu.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://obk.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://ctg.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://pfx.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svx.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xjd.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://ijc.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://ogb.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://gko.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://ogs.fengsongda.top

[J07] 比较两个日期
来源：http://eld.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://xpu.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jkd.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://mlh.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eqi.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://efn.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qnb.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kzb.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://jwr.uphjek.com

[J08] 提取年月日与星期
来源：http://vwm.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://adl.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://udx.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bjn.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kbl.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkw.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vse.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tfm.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rph.sweek.top

[J09] 时区处理
来源：http://ykw.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://keq.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://let.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gyh.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://egg.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dyl.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhs.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ufh.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wds.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://igz.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jzw.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://urd.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uch.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yib.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sge.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ekm.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mcc.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nzl.fanxiaobao.xyz

================================================================================
来源：http://ipe.fanxiaobao.xyz

K. JSON 与序列化
来源：http://int.316326.xyz

================================================================================
来源：http://ajs.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://oof.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mmd.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rrj.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://gje.pycfn.com

TS:   JSON.stringify(obj)
来源：http://yld.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yjs.uphjek.com

Go:   json.Marshal(obj)
来源：http://jah.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://zyg.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fql.yonumen.top

[K02] JSON 字符串转对象
来源：http://xdp.cucudq.cn

Py:   json.loads(s)
来源：http://jju.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dmc.xziqi.cn

JS:   JSON.parse(s)
来源：http://jkk.c1oappe.top

TS:   JSON.parse(s)
来源：http://pcp.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bsk.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://wmx.shuidangran.top

Ruby: JSON.parse(s)
来源：http://kvz.jiagoushi.top


<!-- 参考信息 -->