代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://lff.smart0.xyz

Java: record User(String name, int age) {}
来源：http://zoa.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://ydi.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kuy.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://fsj.dianchejie.cn

[G15] 枚举
来源：http://ail.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ynj.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://huk.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ymb.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lut.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://fct.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qeg.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://cbm.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hjh.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://drb.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://onu.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://tif.hesvh.cn

JS:   Object.entries(obj)
来源：http://vpt.yuanzhike.top

TS:   Object.entries(obj)
来源：http://jlo.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ext.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://osp.yuanzhike.top

Ruby: obj.instance_variables
来源：http://pno.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://vbd.zdbjq.cn

================================================================================
来源：http://wzp.fktsv.cn

H. 异常与错误处理
来源：http://lrr.hywenlv.cn

================================================================================
来源：http://rxi.jiagoushi.top

[H01] try / catch 基础
来源：http://unt.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hbg.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iuh.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tul.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://klf.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cyi.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ukp.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gxq.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nyn.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://wcx.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nnt.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kuh.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vzb.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mkm.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://mpo.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cph.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kcf.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dto.shzxlz.cn

[H03] 主动抛出异常
来源：http://eyr.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://vbv.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rdk.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://fjy.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://mbu.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://yrh.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zyl.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yep.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://mia.yonumen.top

[H04] 自定义异常类型
来源：http://qle.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://nqp.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zpx.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://emw.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://daz.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://bya.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bfx.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://twz.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://tqu.andypj.xyz

[H05] 捕获特定类型
来源：http://zuw.yj202588.top

Py:   except ValueError as e:
来源：http://fkn.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tip.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://uiw.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://yne.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fvk.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bni.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://tzf.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rej.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://rji.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://qrg.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://har.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://kba.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jrv.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dgl.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dhf.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://sbn.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://odu.xuanzx.com

[H07] 断言
来源：http://kuy.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://kzk.ybcxt.top

PHP:  assert($x > 0);
来源：http://lcb.316326.xyz

JS:   console.assert(x > 0);
来源：http://fhh.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://shm.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://pcf.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vjp.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://fmm.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://diy.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://slb.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://kaf.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ggt.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://mkb.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://vkz.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://whr.vehdjk.com

Go:   err.Error()
来源：http://zja.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://hpn.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://mdh.bbcook.cn

[H09] 带错误码的异常
来源：http://tvn.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://flf.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://omo.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ale.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcq.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eed.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://utl.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eos.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zmt.dianchejie.cn

[H10] 资源自动释放
来源：http://ytf.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hkv.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qlf.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jgj.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bne.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bgz.yj20258888.top

Go:   defer f.Close()
来源：http://dow.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://opu.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tlf.tanke756.top

================================================================================
来源：http://anj.shuidangran.top

I. 正则表达式
来源：http://vhq.ywan-chungtsiang.top

================================================================================
来源：http://lmc.hysaishi.cn

[I01] 判断是否匹配
来源：http://hyr.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kim.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ovo.yj20258888.top

JS:   /\d+/.test(s)
来源：http://ugn.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://oqj.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jbr.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ylp.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://eto.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xbn.tanke756.top

[I02] 提取所有匹配
来源：http://awp.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://dye.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://epq.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nht.havefunace.top

TS:   s.match(/\d+/g)
来源：http://pcn.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dfr.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://juo.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://hxl.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezd.xuanzx.com

[I03] 提取捕获分组
来源：http://xie.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hbr.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://grf.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vwz.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wtx.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cge.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwb.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vfk.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://psv.hysaishi.cn

[I04] 正则替换
来源：http://qct.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qbl.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ejn.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://lqs.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wxe.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://mud.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ehj.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://szl.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfc.redwolf501.top

[I05] 按正则拆分
来源：http://hmz.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eaz.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lgl.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://ujo.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://sga.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://mkn.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gvy.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cvb.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lez.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxm.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://avw.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vin.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvx.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvd.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hio.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igg.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vdw.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jyg.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://rps.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aow.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aro.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ios.chenlongwang.top

TS:   /error/gim
来源：http://zfs.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tpu.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cyz.sweek.top

Ruby: s.scan(/error/i)
来源：http://kta.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ohx.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://zmx.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uqt.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ekc.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybd.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wch.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://inu.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dsv.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ncf.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ewi.zhoulong.xyz

================================================================================
来源：http://eaw.gaohongyu789.top

J. 日期与时间
来源：http://put.andypj.xyz

================================================================================
来源：http://gaq.zhengqikj.top

[J01] 获取当前时间
来源：http://sax.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://clg.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kfl.yvedp.cn

JS:   new Date();  Date.now()
来源：http://ocy.bjfxy.top

TS:   new Date();  Date.now()
来源：http://dyj.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ibc.nanxinkj.top

Go:   time.Now()
来源：http://kvy.nanxuanxn.top

Ruby: Time.now
来源：http://bnw.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mrz.nanxuanxn.top

[J02] 格式化输出
来源：http://vku.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgf.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xnh.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gyx.tarul.cn

TS:   d.toISOString()
来源：http://pgl.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pdt.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fzd.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brn.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://frl.yongpay.top

[J03] 字符串解析为日期
来源：http://mpu.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gvz.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqn.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://ied.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://wcy.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://fah.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://spt.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://bpv.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hmt.c1oappe.top

[J04] 时间戳与日期互转
来源：http://xla.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kda.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uef.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tpz.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://evw.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dyk.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qni.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yyc.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zzn.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://vno.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://kkk.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hlu.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gih.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://htt.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://krn.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://alr.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://rwk.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bfp.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://nlo.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://htx.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://pex.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pcm.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://swf.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://hcq.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://eme.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://xty.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://aeq.havefunace.top

[J07] 比较两个日期
来源：http://obd.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ytt.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gjm.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wvw.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fjf.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://let.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dgi.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fyo.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://jdw.hysaishi.cn

[J08] 提取年月日与星期
来源：http://exv.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://igj.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://abw.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lfh.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pqj.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nkf.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oaa.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://llo.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cwg.xuetiantiany.cn

[J09] 时区处理
来源：http://wqy.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mcf.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xoj.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pct.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qfh.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vma.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://byp.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xgo.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://clo.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://oog.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jsf.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ypu.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gpm.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qjp.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jxo.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hsz.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rac.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fuj.jinyuanbaomall.cn

================================================================================
来源：http://yew.xziqi.cn

K. JSON 与序列化
来源：http://bjf.yangfankeji.com

================================================================================
来源：http://prp.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://jpr.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eza.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wtd.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://uoo.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://kce.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kgc.smart0.xyz

Go:   json.Marshal(obj)
来源：http://jng.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lbp.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qsm.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://lqf.ydjk.org.cn

Py:   json.loads(s)
来源：http://qth.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cik.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://ixg.sweek.top


<!-- 参考信息 -->