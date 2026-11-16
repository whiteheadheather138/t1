代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://opn.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://wyn.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://mfj.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jje.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://ktn.hysaishi.cn

[G15] 枚举
来源：http://nit.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oaz.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://usi.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dye.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://grs.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://thn.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fis.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://kin.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eed.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://fzf.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fxx.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://ycw.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://vcl.hnqzz.top

TS:   Object.entries(obj)
来源：http://sia.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ujw.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://euu.yj20258.top

Ruby: obj.instance_variables
来源：http://tes.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://ibu.dashuyun.cn

================================================================================
来源：http://sck.9152youxi.cn

H. 异常与错误处理
来源：http://ghq.haohaochexian.top

================================================================================
来源：http://lto.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://xbi.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://usd.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lfy.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kwt.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://weu.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jey.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://glr.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kks.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rqk.xinyue.icu

[H02] finally / ensure 收尾
来源：http://xap.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://vbc.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://uhv.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bjm.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nde.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ntk.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vfd.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kee.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sja.yanxiufei.cn

[H03] 主动抛出异常
来源：http://ouv.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://aqj.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgh.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://ekb.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://ymr.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lnt.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxu.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eij.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xqd.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://rax.316326.xyz

Py:   class MyError(Exception): pass
来源：http://ece.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oae.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://qqb.yvedp.cn

TS:   class MyError extends Error {}
来源：http://ulj.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://mol.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kct.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://kpa.bbcook.cn

C#:   class MyException : Exception {}
来源：http://xmz.yvedp.cn

[H05] 捕获特定类型
来源：http://jkh.jinqigfzy.top

Py:   except ValueError as e:
来源：http://hon.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kgl.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://bkc.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://bju.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://uix.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zkt.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://zdm.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jmj.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://owz.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://cya.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xgt.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://vgg.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://dmf.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xim.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gwd.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://ewl.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://hsl.pycfn.com

[H07] 断言
来源：http://hqm.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://kvg.chenlongwang.top

PHP:  assert($x > 0);
来源：http://mvl.xziqi.cn

JS:   console.assert(x > 0);
来源：http://ezn.sweek.top

TS:   console.assert(x > 0);
来源：http://vqt.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://hhr.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xye.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://now.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://biy.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://itv.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://ygi.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ukq.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://cta.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jsm.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dbc.haohaochexian.top

Go:   err.Error()
来源：http://hto.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://itb.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://rvm.ctjpmb.com

[H09] 带错误码的异常
来源：http://lbj.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wuf.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://haz.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rly.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lru.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://upq.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hoc.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dzj.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tcn.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://wdo.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkr.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dbu.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wpo.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qjd.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gdv.jlsjyb.cn

Go:   defer f.Close()
来源：http://xao.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ztv.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qqw.uphjek.com

================================================================================
来源：http://chx.jinqigufen.top

I. 正则表达式
来源：http://ypd.ppjwa.cn

================================================================================
来源：http://jed.havefunace.top

[I01] 判断是否匹配
来源：http://uqj.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hkb.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bns.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://cvt.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://pjv.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xld.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xgu.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://ghb.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ltt.jqgfzy.top

[I02] 提取所有匹配
来源：http://zlg.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://xdu.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eqp.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xcy.cashguo.top

TS:   s.match(/\d+/g)
来源：http://xux.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qqb.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://scx.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://pef.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://try.tarul.cn

[I03] 提取捕获分组
来源：http://cph.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://afd.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hte.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://and.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lmh.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lcm.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ntj.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jmg.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bwy.yj202588.top

[I04] 正则替换
来源：http://cgm.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sxz.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eaj.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wmf.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gwq.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://hsf.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pou.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qbx.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ccs.daxiang520.top

[I05] 按正则拆分
来源：http://khb.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yox.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdt.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://kmz.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://gyf.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://abt.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rgr.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qlp.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mmn.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qak.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kfc.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hqm.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://atd.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://plh.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cmk.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lvx.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vse.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tkh.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://ytu.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hko.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pmn.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uad.yueranfly.top

TS:   /error/gim
来源：http://bzn.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vqn.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hxr.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://uup.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xic.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://nly.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejy.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://prb.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqd.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lsw.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ggq.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://prj.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aec.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cfa.fanxiaobao.xyz

================================================================================
来源：http://fva.cucudq.cn

J. 日期与时间
来源：http://qep.jlsjyb.cn

================================================================================
来源：http://pxz.chenjidiqi.icu

[J01] 获取当前时间
来源：http://bgr.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://azw.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kmj.zycfv.cn

JS:   new Date();  Date.now()
来源：http://oyb.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://xyz.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fhe.ivvv.top

Go:   time.Now()
来源：http://lop.sxryk.cn

Ruby: Time.now
来源：http://yvm.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ghq.jinqigfzy.top

[J02] 格式化输出
来源：http://vcd.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qgz.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dua.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ecy.yongpay.top

TS:   d.toISOString()
来源：http://znj.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zdr.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qjk.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mst.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ztw.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://jtg.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gtz.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tug.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://nar.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://iaa.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://pja.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vuf.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://xko.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pxz.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://tyv.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ard.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://luv.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kvj.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hju.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bvf.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gey.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qzc.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wzm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://pbe.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://ocr.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gmn.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sbq.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://red.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://ybb.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtb.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://fya.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ibh.yj20258888.top

[J06] 计算两时间之差
来源：http://isv.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://qzf.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://eou.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://apj.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jdg.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://jah.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://tja.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://huz.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://pdu.pycfn.com

[J07] 比较两个日期
来源：http://zle.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bdb.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cyc.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fzi.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vyw.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfl.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pov.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://poe.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://oea.dashuyun.cn

[J08] 提取年月日与星期
来源：http://jyz.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ecv.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jjx.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blj.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uno.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://laz.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uxe.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gkt.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dlz.fktsv.cn

[J09] 时区处理
来源：http://yhv.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wcb.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qer.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xcp.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jih.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mcy.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hcl.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iry.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://plx.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://htv.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mqd.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lwm.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qyy.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rbe.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnz.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gup.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ulr.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://acr.ehwqpu.com

================================================================================
来源：http://ezv.shanyushiyangtech.top

K. JSON 与序列化
来源：http://xjb.zycfv.cn

================================================================================
来源：http://dcd.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://mum.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mbs.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odb.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://tul.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://kln.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kaa.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://jip.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://lrn.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://uzx.daria6918.cn

[K02] JSON 字符串转对象
来源：http://bey.pycfn.com

Py:   json.loads(s)
来源：http://btx.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://owi.chenzaomai.com

JS:   JSON.parse(s)
来源：http://ine.xuanzx.com


<!-- 参考信息 -->