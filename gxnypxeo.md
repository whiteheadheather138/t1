代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wzz.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tiq.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://gpl.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dye.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://eth.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ext.yj202588.top

[G16] 对象转数组 / 字典
来源：http://pwg.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://haf.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://vhm.dianchejie.cn

JS:   Object.entries(obj)
来源：http://bub.sxryk.cn

TS:   Object.entries(obj)
来源：http://sys.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fxv.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eap.shzxlz.cn

Ruby: obj.instance_variables
来源：http://buu.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://sol.hcnkem.com

================================================================================
来源：http://hti.cashguo.top

H. 异常与错误处理
来源：http://zbr.hammf.cn

================================================================================
来源：http://yfb.birdmap.top

[H01] try / catch 基础
来源：http://gth.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pfn.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ouo.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://haj.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uxv.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://off.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uoh.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gqc.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsw.wangdashe.top

[H02] finally / ensure 收尾
来源：http://qsh.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tdq.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rsz.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://kmt.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oet.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kga.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fbp.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://klk.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iti.snrcjt.cn

[H03] 主动抛出异常
来源：http://gfz.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://emb.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xax.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://tns.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://dhj.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hlv.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ang.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fyf.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://dyw.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://hca.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://pyr.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://ouj.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://veo.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://nnh.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://bpp.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zxd.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://shi.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://ckp.yvedp.cn

[H05] 捕获特定类型
来源：http://kkj.zhijiandao.cn

Py:   except ValueError as e:
来源：http://wry.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nvb.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://nlw.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://xxn.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://zxv.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://szy.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://vud.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rzh.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://fqn.daria6918.cn

Py:   value = d.get("k") or default
来源：http://mzm.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://taa.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://bss.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://uzu.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmt.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dlu.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://xvk.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://vru.guannengcc.top

[H07] 断言
来源：http://knx.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://rnk.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://opg.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://gwn.daria6918.cn

TS:   console.assert(x > 0);
来源：http://iem.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://bwb.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sti.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://jlc.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://eqx.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://qhj.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://sno.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://awh.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://umg.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ooh.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fzk.jqgufenzy.top

Go:   err.Error()
来源：http://lqq.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://xgr.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://xsm.0kj1m.cn

[H09] 带错误码的异常
来源：http://qbn.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rcb.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://war.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eks.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xcs.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ial.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqu.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jdk.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bdf.hnqzz.top

[H10] 资源自动释放
来源：http://cym.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mhg.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://evm.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://waa.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kwa.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ssc.yuanzhike.top

Go:   defer f.Close()
来源：http://yqq.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jop.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wem.fktsv.cn

================================================================================
来源：http://vcb.yonumen.top

I. 正则表达式
来源：http://kau.ctjpmb.com

================================================================================
来源：http://qcg.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://ium.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kin.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kwb.tarul.cn

JS:   /\d+/.test(s)
来源：http://usv.316326.xyz

TS:   /\d+/.test(s)
来源：http://bld.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tcx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfv.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://uov.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ird.svipenyu.cn

[I02] 提取所有匹配
来源：http://dnc.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://prq.fanxiaobao.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hwe.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iks.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://xut.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nqp.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zva.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://zmu.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ero.yongpay.top

[I03] 提取捕获分组
来源：http://ddh.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lgq.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://brn.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qee.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zdp.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tml.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ztw.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jyh.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhf.yonumen.top

[I04] 正则替换
来源：http://jtr.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ioy.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hkz.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://xvo.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hqz.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://bvo.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hgi.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pxi.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mcq.aizwys.cn

[I05] 按正则拆分
来源：http://kxc.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fxs.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aus.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://ojm.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://hmg.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://mkf.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://psp.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://hdw.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jpr.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mjr.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zvy.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iug.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mts.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fnk.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kgm.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ejd.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfl.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://siy.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://qrc.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tzs.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ujp.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rkt.mhx1999.top

TS:   /error/gim
来源：http://anq.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tpg.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hqk.ivvv.top

Ruby: s.scan(/error/i)
来源：http://dqg.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iqh.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://hmx.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cdk.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nek.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://whr.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbq.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zqp.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cbi.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://reh.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://olt.jqgfzy.top

================================================================================
来源：http://ghu.jianghu66.top

J. 日期与时间
来源：http://ghj.wangshuangyany.cn

================================================================================
来源：http://avg.vehdjk.com

[J01] 获取当前时间
来源：http://nbp.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eyx.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cdx.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://orn.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://vxo.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aro.guowangkeji.top

Go:   time.Now()
来源：http://emg.daria6918.cn

Ruby: Time.now
来源：http://nmm.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ozx.dashuyun.cn

[J02] 格式化输出
来源：http://idw.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpn.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xrq.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lgm.zdqjudy.top

TS:   d.toISOString()
来源：http://dvu.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dgc.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qma.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fwh.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yba.gogol.net.cn

[J03] 字符串解析为日期
来源：http://lcj.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xjb.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ewi.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://ufb.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://byr.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://lay.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tdn.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://jyx.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://juj.mhx1999.top

[J04] 时间戳与日期互转
来源：http://wjv.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://frx.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rfl.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iqn.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://pmn.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fqv.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kmx.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vqd.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wgc.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://som.hammf.cn

Py:   now + timedelta(days=7)
来源：http://vix.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bas.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://owj.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kzq.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://uve.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zig.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://mkq.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://utv.epnwcf.com

[J06] 计算两时间之差
来源：http://mdd.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://eol.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://zdp.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wla.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uqo.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://oda.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://oot.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://fhx.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://hsb.hywenlv.cn

[J07] 比较两个日期
来源：http://yga.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://zva.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jgb.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qwy.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://pbq.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zmj.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vus.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://qnu.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://chl.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://bgw.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hyw.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ngy.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://osp.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dfu.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ydr.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rbp.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jbi.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glo.shangyingyoupin.top

[J09] 时区处理
来源：http://raj.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xkm.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ixp.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hok.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qei.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qpc.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://azf.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://enc.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yfo.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://kjw.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vke.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://avf.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvl.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gso.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hkp.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rpo.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://twn.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sse.cqqwz.cn

================================================================================
来源：http://vgo.hesvh.cn

K. JSON 与序列化
来源：http://shn.chenjidiqi.icu

================================================================================
来源：http://oro.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://fhh.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vtf.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vqi.tanke756.top

JS:   JSON.stringify(obj)
来源：http://evc.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://bvu.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://enj.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://ijs.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rib.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wxo.yuxming.cn

[K02] JSON 字符串转对象
来源：http://fuq.sxryk.cn

Py:   json.loads(s)
来源：http://ddi.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yeo.meibo888.top

JS:   JSON.parse(s)
来源：http://taw.ctjpmb.com

TS:   JSON.parse(s)
来源：http://fhk.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bwe.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://pbx.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://phk.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lit.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://ocl.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mzh.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zuy.yonumen.top


<!-- 参考信息 -->