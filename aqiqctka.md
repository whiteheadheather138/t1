代发 wailian999

Py:   isinstance(u, User)
来源：http://ydh.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://fsf.tian-w.cn

JS:   u instanceof User
来源：http://fzk.hammf.cn

TS:   u instanceof User
来源：http://doh.meibo888.top

Java: u instanceof User
来源：http://ayc.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kkp.hesvh.cn

Ruby: u.is_a?(User)
来源：http://lpo.guowangkeji.top

C#:   u is User
来源：http://lus.jqgfzy.top

[G14] 数据类 / record
来源：http://fum.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qlh.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://rrm.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://fiw.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://sqn.hcnkem.com

Java: record User(String name, int age) {}
来源：http://szv.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://yxk.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aym.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://dqv.dianchejie.cn

[G15] 枚举
来源：http://jsq.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://haj.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpf.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rly.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nwh.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://mfh.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sbb.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://xxi.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zbx.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://pat.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cwg.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://ljz.xuanzx.com

JS:   Object.entries(obj)
来源：http://biq.cheryme.top

TS:   Object.entries(obj)
来源：http://yiy.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tam.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tbu.svipenyu.cn

Ruby: obj.instance_variables
来源：http://kou.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://ouc.jqgufenzy.top

================================================================================
来源：http://qse.nanxinkj.top

H. 异常与错误处理
来源：http://fqh.cheryme.top

================================================================================
来源：http://kip.cdnleiting.top

[H01] try / catch 基础
来源：http://uvp.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cso.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iix.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://svn.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sqc.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fqk.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vbp.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://voa.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://onu.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://hvd.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bun.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pcf.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://nnu.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oiy.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://gnr.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cgn.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://afp.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ucc.zhixingplan.top

[H03] 主动抛出异常
来源：http://arp.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://egy.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tky.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://ktk.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://wcv.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://yqn.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qfo.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://iik.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://pwr.jyoumei.cn

[H04] 自定义异常类型
来源：http://zzo.sweek.top

Py:   class MyError(Exception): pass
来源：http://aeu.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wse.xylfe.cn

JS:   class MyError extends Error {}
来源：http://njj.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://imv.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://hat.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ywy.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://wxa.mhx1999.top

C#:   class MyException : Exception {}
来源：http://fhs.yuanzhike.top

[H05] 捕获特定类型
来源：http://gab.yongpay.top

Py:   except ValueError as e:
来源：http://vng.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rqd.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://bpe.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://fqx.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://unu.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://smp.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://mlm.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zbo.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://tiq.iojbl.cn

Py:   value = d.get("k") or default
来源：http://lah.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://osf.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://hqn.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://itd.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eei.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jcg.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://svo.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://gyz.ybcxt.top

[H07] 断言
来源：http://mee.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://zom.jqgfzy.top

PHP:  assert($x > 0);
来源：http://jin.fehbvm.com

JS:   console.assert(x > 0);
来源：http://xya.yuxming.cn

TS:   console.assert(x > 0);
来源：http://tvx.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://wqt.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mnj.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://qsh.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://tvn.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://shy.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://ndd.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mvn.meibo888.top

JS:   e.message;  e.stack
来源：http://weg.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lgk.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fjn.tarul.cn

Go:   err.Error()
来源：http://xts.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://hmn.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://zlu.hcnkem.com

[H09] 带错误码的异常
来源：http://gld.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nns.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ajq.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hwz.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://awa.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxd.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zto.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://rmi.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ssv.aizwys.cn

[H10] 资源自动释放
来源：http://jwz.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gaz.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tnj.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wbq.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://swd.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bwo.sufxvd.cn

Go:   defer f.Close()
来源：http://key.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lgb.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rmx.fengsongda.top

================================================================================
来源：http://vwt.ydjk.org.cn

I. 正则表达式
来源：http://ruo.nwbrower.top

================================================================================
来源：http://lzi.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://alb.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://por.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://liz.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://vom.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://plj.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fwu.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qdf.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://jke.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ecg.smart0.xyz

[I02] 提取所有匹配
来源：http://zbd.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://dde.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tkc.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sel.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://vea.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://arp.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vkx.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://eix.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yfd.aizwys.cn

[I03] 提取捕获分组
来源：http://bck.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xrc.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fbs.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wrr.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ydl.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gwj.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iwx.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://exf.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gct.havefunace.top

[I04] 正则替换
来源：http://zud.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zpb.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://abq.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://fia.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://jjd.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://hkn.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jbz.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zdx.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nye.fengsongda.top

[I05] 按正则拆分
来源：http://kqy.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cnm.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ngz.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://vox.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://lur.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://ddn.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://udh.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://ygb.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wja.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lpl.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqr.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nha.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://adc.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qfq.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vej.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxt.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yxg.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dup.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://sjo.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://azj.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ctn.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rod.xziqi.cn

TS:   /error/gim
来源：http://ukq.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fdc.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aog.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://uth.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wfu.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zyw.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bpv.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xlk.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dar.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oko.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://icc.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ebg.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://egi.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nya.shuidangran.top

================================================================================
来源：http://lxb.ydjk.org.cn

J. 日期与时间
来源：http://qre.yangfankeji.com

================================================================================
来源：http://rej.jqgufenzy.top

[J01] 获取当前时间
来源：http://qhi.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gbs.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yvv.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://sof.sxryk.cn

TS:   new Date();  Date.now()
来源：http://uvj.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bea.fehbvm.com

Go:   time.Now()
来源：http://ony.pycfn.com

Ruby: Time.now
来源：http://hng.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zrq.ivvv.top

[J02] 格式化输出
来源：http://drd.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oeg.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bgj.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mhj.yanxiufei.cn

TS:   d.toISOString()
来源：http://csd.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uqm.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wjf.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqr.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xfc.ybcxt.top

[J03] 字符串解析为日期
来源：http://zbr.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pqe.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xoh.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://jox.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://ehm.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://cvh.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jtx.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://kdc.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://caf.c1oappe.top

[J04] 时间戳与日期互转
来源：http://une.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vwu.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qtg.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mgk.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vav.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bwf.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gve.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iuf.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eqh.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://lqe.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://mye.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://afk.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cez.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfr.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://paa.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pnr.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://ptb.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rin.uphjek.com

[J06] 计算两时间之差
来源：http://ojt.birdmap.top

Py:   (end - start).total_seconds()
来源：http://kan.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://ztr.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://njq.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pfs.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://fup.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://tcc.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://ahu.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://esp.jyoumei.cn

[J07] 比较两个日期
来源：http://jxn.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://end.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hay.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://wax.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://xkv.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vsr.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwb.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://hlz.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://bla.yueranfly.top

[J08] 提取年月日与星期
来源：http://pwn.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kxl.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vgk.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gpk.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xqh.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dty.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pvj.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sda.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wpn.yanxiufei.cn

[J09] 时区处理
来源：http://foo.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mij.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bbi.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbh.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mcl.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zbv.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://opa.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dph.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mml.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://rlf.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://chw.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tah.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zhz.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://muf.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://izk.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ytr.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fxo.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cyd.hammf.cn

================================================================================
来源：http://oue.tarul.cn

K. JSON 与序列化
来源：http://qqg.gaohongyu789.top

================================================================================
来源：http://fxt.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://mdh.xuanzx.com


<!-- 参考信息 -->