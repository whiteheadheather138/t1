代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vdv.gotoacloud.top

[G15] 枚举
来源：http://odt.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fnx.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jqk.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ykf.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kkz.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://mpb.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vep.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://fqw.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xkx.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://gvj.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ddm.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://ddx.nwbrower.top

JS:   Object.entries(obj)
来源：http://pdc.bbcook.cn

TS:   Object.entries(obj)
来源：http://wql.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uyv.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://eqj.hcnkem.com

Ruby: obj.instance_variables
来源：http://lta.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://uei.fzhhl.top

================================================================================
来源：http://vlu.yvedp.cn

H. 异常与错误处理
来源：http://bwm.c1oappe.top

================================================================================
来源：http://fso.yongpay.top

[H01] try / catch 基础
来源：http://eek.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sjg.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sfl.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qdv.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oqo.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://som.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yjw.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qsa.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rah.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://nzm.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://ske.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://bcx.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jwm.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xdq.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://ugk.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hyy.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nin.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vgw.jqgufenzy.top

[H03] 主动抛出异常
来源：http://suj.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://ftu.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwa.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://lbq.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://otm.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ona.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wct.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://tpw.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hkf.zycfv.cn

[H04] 自定义异常类型
来源：http://hhs.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://glz.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://zsi.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://fmv.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://nma.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://hsf.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kna.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://urr.tian-w.cn

C#:   class MyException : Exception {}
来源：http://rjb.chenlongwang.top

[H05] 捕获特定类型
来源：http://fpp.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://dai.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sgs.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://rtj.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://qoe.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://zbz.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zuw.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://mzm.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xuc.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://kcp.hcnkem.com

Py:   value = d.get("k") or default
来源：http://hve.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://bvy.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fqe.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://acn.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://was.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mhe.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://vez.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://cqh.gzhubu.top

[H07] 断言
来源：http://mfr.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://ssn.dashuyun.cn

PHP:  assert($x > 0);
来源：http://oet.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://rrk.cheryme.top

TS:   console.assert(x > 0);
来源：http://cfy.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://kap.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://slx.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://trd.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://zpr.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://xzq.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://rrx.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rfv.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://cta.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ran.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://efm.jqgufenzy.top

Go:   err.Error()
来源：http://muf.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://vtp.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://rlr.jlsjyb.cn

[H09] 带错误码的异常
来源：http://vrh.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bnm.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hlg.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://plj.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vyp.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://clc.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nyg.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://tzo.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bqx.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://dlk.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://smj.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lws.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wwe.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ply.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zyt.redwolf501.top

Go:   defer f.Close()
来源：http://jpf.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rpx.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tal.52xcode.cn

================================================================================
来源：http://fud.smart0.xyz

I. 正则表达式
来源：http://cme.cdnleiting.top

================================================================================
来源：http://xlo.yj20258.top

[I01] 判断是否匹配
来源：http://qqv.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wkp.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://yqn.yonumen.top

JS:   /\d+/.test(s)
来源：http://zra.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://tob.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jzf.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nem.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://ckm.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nww.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://gui.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://jqa.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ucq.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hbc.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://vcn.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://izo.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://koy.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://mfh.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://snk.nwbrower.top

[I03] 提取捕获分组
来源：http://plh.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aqt.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ovo.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mso.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hil.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pmd.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://evd.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://egv.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sct.sysykeji.top

[I04] 正则替换
来源：http://vdj.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tlo.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://osq.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://tng.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://nre.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://hvt.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fqw.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nxg.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ajn.yj202588.top

[I05] 按正则拆分
来源：http://bjd.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mjd.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mrd.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://qfr.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://xfe.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://sqi.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ouc.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://xki.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oev.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fzi.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zwz.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://liw.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://znl.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pcw.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fkd.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dos.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xms.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fdx.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://spj.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byn.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dzp.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jru.svipenyu.cn

TS:   /error/gim
来源：http://aoy.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fny.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aev.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://cry.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zmy.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://nyc.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://erm.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nmv.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvq.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kvq.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zry.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pds.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ziq.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hzw.daria6918.cn

================================================================================
来源：http://aba.jinghuilouyu.cn

J. 日期与时间
来源：http://qtg.chenjidiqi.icu

================================================================================
来源：http://ikn.cheryme.top

[J01] 获取当前时间
来源：http://grl.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://cro.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sue.cashguo.top

JS:   new Date();  Date.now()
来源：http://mrv.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://ywi.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yag.fzhhl.top

Go:   time.Now()
来源：http://thl.kuanghao11.cn

Ruby: Time.now
来源：http://gcn.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vic.andypj.xyz

[J02] 格式化输出
来源：http://gsg.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tdz.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ufp.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://flr.redwolf501.top

TS:   d.toISOString()
来源：http://lgy.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fbn.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iro.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fur.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tuy.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://pfe.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jmp.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://icz.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://omm.yongpay.top

TS:   new Date("2024-01-02")
来源：http://qhz.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://naf.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yfd.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://elv.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldn.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://fat.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gae.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oqf.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yde.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tmo.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rjr.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sze.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sog.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xwv.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://kng.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://rdg.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://url.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpn.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zfl.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://zpm.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wkh.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://anu.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://cxc.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://zmc.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://gpj.sweek.top

PHP:  $end->diff($start)->days;
来源：http://mdx.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://han.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gtr.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fsc.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://ddr.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://cqo.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://tlc.nanxuanxn.top

[J07] 比较两个日期
来源：http://ydk.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://kry.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zwp.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://yru.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iye.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qlo.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qfd.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://mhj.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://efz.xziqi.cn

[J08] 提取年月日与星期
来源：http://bmt.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbj.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fsy.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vcw.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://twx.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gvn.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://afv.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfl.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tpy.chenjidiqi.icu

[J09] 时区处理
来源：http://ozh.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nuq.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://azq.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywu.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hzo.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xje.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bmq.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vhm.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hrt.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://yxw.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cyx.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qkz.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsu.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrq.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okd.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ywt.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kgo.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ama.kuanghao11.cn

================================================================================
来源：http://grw.fktsv.cn

K. JSON 与序列化
来源：http://vyr.cdnleiting.top

================================================================================
来源：http://ydk.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://tpb.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ufp.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vtw.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://uin.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://hct.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bku.epnwcf.com

Go:   json.Marshal(obj)
来源：http://vcf.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ocr.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bgg.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://frr.sufxvd.cn

Py:   json.loads(s)
来源：http://djv.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dsf.zhengqikj.top

JS:   JSON.parse(s)
来源：http://wrd.yj202588.top

TS:   JSON.parse(s)
来源：http://emw.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://atc.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://qtx.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://vnn.cashguo.top


<!-- 参考信息 -->