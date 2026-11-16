代发 wailian999

C#:   record User(string Name, int Age);
来源：http://ytx.hnxiangtu.top

[G15] 枚举
来源：http://arm.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://niv.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://nca.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://joy.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mad.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://yiv.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ntf.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://rbj.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rpx.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://gxb.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kmy.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://tfa.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://kva.hnqzz.top

TS:   Object.entries(obj)
来源：http://bkk.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nrb.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://krd.haohaochexian.top

Ruby: obj.instance_variables
来源：http://spp.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://xqz.fengsongda.top

================================================================================
来源：http://yyv.zdbjq.cn

H. 异常与错误处理
来源：http://guo.tianlin.xyz

================================================================================
来源：http://mdb.zycfv.cn

[H01] try / catch 基础
来源：http://imt.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://msg.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lhp.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lsv.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qby.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgr.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nzs.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ykc.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zxw.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://esb.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hde.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hln.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://djm.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yrn.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://heo.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wru.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vjp.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yrp.zhengqikj.top

[H03] 主动抛出异常
来源：http://rdj.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://wav.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kct.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://kof.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://mtx.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nuo.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rya.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dli.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://spu.gaohongyu789.top

[H04] 自定义异常类型
来源：http://ilm.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://yvb.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://yzd.yongpay.top

JS:   class MyError extends Error {}
来源：http://fvp.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://qxz.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://jkt.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pse.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://wqu.bbcook.cn

C#:   class MyException : Exception {}
来源：http://trp.jinqigufen.top

[H05] 捕获特定类型
来源：http://tjx.daxiang520.top

Py:   except ValueError as e:
来源：http://ojf.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pkf.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://qug.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://uks.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://cpd.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yah.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://gxm.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://amp.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://gcj.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://xwh.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://onz.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hjj.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://zuh.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cfb.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mtj.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://afc.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://naa.pengpengdd.cyou

[H07] 断言
来源：http://rby.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://sis.yuanzhike.top

PHP:  assert($x > 0);
来源：http://jgd.ydzc1.top

JS:   console.assert(x > 0);
来源：http://inb.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://ndt.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://ary.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ozs.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://dbl.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://jmy.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://trh.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://fys.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vyc.fengsongda.top

JS:   e.message;  e.stack
来源：http://oka.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wdh.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cah.mhx1999.top

Go:   err.Error()
来源：http://hnl.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://kbi.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://myf.zdqjudy.top

[H09] 带错误码的异常
来源：http://nzr.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tzf.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://max.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rug.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gxz.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hxb.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rso.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://wxw.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cmf.chenzaomai.com

[H10] 资源自动释放
来源：http://isv.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://skt.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://inu.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://czo.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rca.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://att.hesvh.cn

Go:   defer f.Close()
来源：http://lhc.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kzn.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://snz.yuxming.cn

================================================================================
来源：http://bcn.hesvh.cn

I. 正则表达式
来源：http://kbe.shanyushiyangkeji.top

================================================================================
来源：http://ccr.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://lvr.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://trw.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://zzh.iojbl.cn

JS:   /\d+/.test(s)
来源：http://ryq.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://oqq.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iis.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://exh.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://vvf.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vro.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://mwi.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://xek.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ahv.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yee.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://mzd.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qkg.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ssx.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://tfq.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://imk.yonumen.top

[I03] 提取捕获分组
来源：http://ezq.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://chg.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://usy.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vul.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ebg.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ixb.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jgz.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wjz.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://had.shzxlz.cn

[I04] 正则替换
来源：http://hzy.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ftb.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tdh.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://ysz.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://nfj.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hkc.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dfh.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dcm.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klm.ivvv.top

[I05] 按正则拆分
来源：http://qlz.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ven.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jcl.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://pgy.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://juy.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://ejl.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zvx.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://oww.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gfq.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://luj.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wgb.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jto.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhd.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqr.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xza.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dtp.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ldr.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hqr.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://lum.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://opd.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vpe.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ykp.zhixingplan.top

TS:   /error/gim
来源：http://msb.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jwn.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://obd.ivvv.top

Ruby: s.scan(/error/i)
来源：http://hjy.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idy.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://jnx.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://des.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ohu.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://euq.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qgj.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xfk.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uqb.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qux.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://epc.9152youxi.cn

================================================================================
来源：http://tcz.cashguo.top

J. 日期与时间
来源：http://isi.smart0.xyz

================================================================================
来源：http://wwr.haohaochexian.top

[J01] 获取当前时间
来源：http://ysj.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cie.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://utx.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://jvd.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://qwk.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://coi.hywenlv.cn

Go:   time.Now()
来源：http://hfy.ydjk.org.cn

Ruby: Time.now
来源：http://iwk.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hqc.xuanzx.com

[J02] 格式化输出
来源：http://vux.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tju.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wte.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cvn.xinyue.icu

TS:   d.toISOString()
来源：http://qqm.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gyt.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nze.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://utr.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://itz.mhx1999.top

[J03] 字符串解析为日期
来源：http://rkp.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wtt.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://muj.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://awz.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://ati.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://caz.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bpz.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ore.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iur.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://nhi.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hsg.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qqp.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://okk.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://msw.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fjj.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zoj.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bzv.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zco.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://gpp.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://hwk.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yhh.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izf.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://phg.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://ype.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xhd.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://sde.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://idu.jinqigufen.top

[J06] 计算两时间之差
来源：http://wxh.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://xey.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://dem.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://afa.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nkv.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://cen.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://fdw.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://ura.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://nbv.gzhubu.top

[J07] 比较两个日期
来源：http://dcb.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://eye.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lja.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hoi.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://the.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://btb.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qrf.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://crd.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://bmp.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://mlg.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ssf.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rok.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vwi.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vcu.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rdn.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dbc.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jfd.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dzj.nanxinkj.top

[J09] 时区处理
来源：http://mjd.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kmr.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://omf.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rls.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdw.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jaf.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nla.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mbs.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xbe.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://oju.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rtq.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xmq.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fqt.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sld.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wnr.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://trf.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://azk.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unf.nanxinkj.top

================================================================================
来源：http://rlm.fanxiaobao.xyz

K. JSON 与序列化
来源：http://rwg.mhx1999.top

================================================================================
来源：http://ybc.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://abw.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nat.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dux.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://ylr.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://csj.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qvh.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://aqs.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fxg.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zzo.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://kbc.tianlin.xyz

Py:   json.loads(s)
来源：http://fbv.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyq.yueranfly.top

JS:   JSON.parse(s)
来源：http://wuq.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://usq.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wmd.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://uie.guannengcc.top

Ruby: JSON.parse(s)
来源：http://oud.tanke756.top


<!-- 参考信息 -->