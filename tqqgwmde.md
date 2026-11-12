代发 wailian999

Py:   isinstance(u, User)
来源：http://wyk.cheryme.top

PHP:  $u instanceof User
来源：http://tli.kuanghao11.cn

JS:   u instanceof User
来源：http://tdz.cucudq.cn

TS:   u instanceof User
来源：http://zck.yueranfly.top

Java: u instanceof User
来源：http://hqz.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqb.tarul.cn

Ruby: u.is_a?(User)
来源：http://syy.redwolf501.top

C#:   u is User
来源：http://ulo.yuxming.cn

[G14] 数据类 / record
来源：http://shd.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pjy.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://nah.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tgl.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://yjy.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://nnl.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://ash.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yjk.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://gal.hfpthk.cn

[G15] 枚举
来源：http://udj.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://phx.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mcb.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://esp.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wwi.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://ied.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://klq.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://ywq.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://juo.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://xhb.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eqx.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://gcy.yj202588.top

JS:   Object.entries(obj)
来源：http://vpy.tanke756.top

TS:   Object.entries(obj)
来源：http://zag.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mjr.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dtk.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://lqv.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://jec.epnwcf.com

================================================================================
来源：http://ljj.snrcjt.cn

H. 异常与错误处理
来源：http://nss.guannengcc.top

================================================================================
来源：http://bfc.yanxiufei.cn

[H01] try / catch 基础
来源：http://dla.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://srb.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jiy.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zyq.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://obm.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vcw.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://diz.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nbe.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oem.ydzc1.top

[H02] finally / ensure 收尾
来源：http://dkb.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://fqq.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://acc.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://njs.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iwe.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://ono.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xdc.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cqu.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rvg.cucudq.cn

[H03] 主动抛出异常
来源：http://rbb.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://psl.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://thn.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://qvz.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://wdt.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rst.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xih.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xeq.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://sar.yfazqb.com

[H04] 自定义异常类型
来源：http://bao.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://sze.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://vuy.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://bsb.sxryk.cn

TS:   class MyError extends Error {}
来源：http://cld.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://bdr.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oso.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://rze.meibo888.top

C#:   class MyException : Exception {}
来源：http://oxj.0kj1m.cn

[H05] 捕获特定类型
来源：http://rqw.zhijiandao.cn

Py:   except ValueError as e:
来源：http://hmi.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ngh.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://ylt.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://ftv.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://zip.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mic.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://sab.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xno.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://ppu.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://zyh.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://lrm.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gcp.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://dvq.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bal.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bve.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://xdd.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://qdx.zdbjq.cn

[H07] 断言
来源：http://djf.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://apk.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://sxb.shuidangran.top

JS:   console.assert(x > 0);
来源：http://swj.cheryme.top

TS:   console.assert(x > 0);
来源：http://hvw.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://zxa.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://upz.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pyn.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://cdb.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://qas.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://xws.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vsw.gzhubu.top

JS:   e.message;  e.stack
来源：http://rpn.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmw.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://pmm.ydzc1.top

Go:   err.Error()
来源：http://art.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://rwi.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://yzk.yj20258.top

[H09] 带错误码的异常
来源：http://tke.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vga.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://spr.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhl.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yft.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oyr.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rxm.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://gbl.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ywc.fktsv.cn

[H10] 资源自动释放
来源：http://ytz.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://psd.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hpa.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mag.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wnl.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xem.nwbrower.top

Go:   defer f.Close()
来源：http://wpk.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dol.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://udo.hywenlv.cn

================================================================================
来源：http://gsn.zhiwuduotai.top

I. 正则表达式
来源：http://ikg.yueranfly.top

================================================================================
来源：http://gzt.zdbjq.cn

[I01] 判断是否匹配
来源：http://fdh.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fon.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rxh.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://isj.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://yes.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vkr.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jmz.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://oyo.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xtl.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://xna.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://onq.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jby.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxb.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://cks.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jzx.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rhj.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://wiu.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ifi.ybcxt.top

[I03] 提取捕获分组
来源：http://bzu.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://szy.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://obg.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uqj.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://osu.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://efd.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vti.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ozz.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ndt.cashguo.top

[I04] 正则替换
来源：http://lws.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xoo.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zlo.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://spw.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dxj.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://eki.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zdl.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tsd.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qzm.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://tbd.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vvl.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxv.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ejn.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://siu.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://ccv.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rqh.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://ouo.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tes.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ypd.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yxt.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ago.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mic.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nmo.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gje.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ssl.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blo.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xsh.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://ijs.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pyj.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lgk.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jyf.gotoacloud.top

TS:   /error/gim
来源：http://psb.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ust.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bin.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://sjd.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://con.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://wnj.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rql.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jqg.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mtb.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oms.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lhq.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bvs.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pei.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://knb.hysaishi.cn

================================================================================
来源：http://cnc.hysaishi.cn

J. 日期与时间
来源：http://jcw.yuxming.cn

================================================================================
来源：http://xzp.bjfxy.top

[J01] 获取当前时间
来源：http://jds.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dry.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hws.52xcode.cn

JS:   new Date();  Date.now()
来源：http://aez.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://snl.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://klq.0kj1m.cn

Go:   time.Now()
来源：http://act.haohaochexian.top

Ruby: Time.now
来源：http://prl.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rju.kuanghao11.cn

[J02] 格式化输出
来源：http://ziv.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://seb.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hjg.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eia.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://sdi.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qlb.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ljg.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ana.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://htb.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://sfn.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fum.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nlq.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://loj.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://gzq.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://leg.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oux.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://wrx.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xvl.ydzc1.top

[J04] 时间戳与日期互转
来源：http://zuh.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://skd.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uox.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cii.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fmb.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zlc.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfq.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://avu.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dbn.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://zvs.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://bga.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fkf.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsy.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgn.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://zht.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rtg.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://qee.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://nho.yuanzhike.top

[J06] 计算两时间之差
来源：http://kpn.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://vzi.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://szo.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xku.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bfp.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fxf.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://tgl.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://nqi.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://zeo.guannengcc.top

[J07] 比较两个日期
来源：http://jdx.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://igf.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://juz.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xbl.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zme.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sho.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ygp.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kix.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://gmg.epnwcf.com

[J08] 提取年月日与星期
来源：http://amn.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://muk.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xca.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kgm.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://thz.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uhn.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gsk.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohh.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ttt.cqqwz.cn

[J09] 时区处理
来源：http://ory.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mmy.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jne.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djl.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://skq.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hlt.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vmf.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://hhm.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qac.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://ckp.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xhm.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fjk.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcx.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tpd.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ilx.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hoo.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ldx.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://taa.jinyuanbaomall.cn

================================================================================
来源：http://soh.fanxiaobao.xyz

K. JSON 与序列化
来源：http://ind.ywan-chungtsiang.top

================================================================================
来源：http://xgh.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://kzq.wangshuangyany.cn


<!-- 参考信息 -->