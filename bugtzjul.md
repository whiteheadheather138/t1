代发 wailian999

Py:   isinstance(u, User)
来源：http://gxa.tianlin.xyz

PHP:  $u instanceof User
来源：http://mle.kuanghao11.cn

JS:   u instanceof User
来源：http://ihc.chenlongwang.top

TS:   u instanceof User
来源：http://may.yuxming.cn

Java: u instanceof User
来源：http://bjf.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sug.zycfv.cn

Ruby: u.is_a?(User)
来源：http://xgz.hywenlv.cn

C#:   u is User
来源：http://fei.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://zva.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://twr.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://ptx.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://dne.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://zqj.pycfn.com

Java: record User(String name, int age) {}
来源：http://orn.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://nux.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbr.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://kbj.shzxlz.cn

[G15] 枚举
来源：http://tpi.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oma.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uwt.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wrf.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npb.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://gqu.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgy.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://kir.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rkf.cashguo.top

[G16] 对象转数组 / 字典
来源：http://wrr.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://axg.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://ujr.havefunace.top

JS:   Object.entries(obj)
来源：http://rjp.cheryme.top

TS:   Object.entries(obj)
来源：http://der.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vri.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rrf.guannengcc.top

Ruby: obj.instance_variables
来源：http://vgv.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://iwe.aizwys.cn

================================================================================
来源：http://cap.redwolf501.top

H. 异常与错误处理
来源：http://dry.gaohongyu789.top

================================================================================
来源：http://mcz.hywenlv.cn

[H01] try / catch 基础
来源：http://kvl.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zjw.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ujz.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vca.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iwj.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mks.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nxn.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xve.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kwb.meibo888.top

[H02] finally / ensure 收尾
来源：http://sne.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://rib.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pfj.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://axz.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pvw.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://ujy.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nhv.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zxp.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wrq.xylfe.cn

[H03] 主动抛出异常
来源：http://pwh.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://flo.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://muj.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://mxt.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://rym.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mon.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://elt.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ogq.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://dea.bjfxy.top

[H04] 自定义异常类型
来源：http://flp.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://cuv.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://wnd.yongpay.top

JS:   class MyError extends Error {}
来源：http://iaq.pycfn.com

TS:   class MyError extends Error {}
来源：http://omc.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://fmd.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blq.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://vel.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://ttf.jianghu66.top

[H05] 捕获特定类型
来源：http://vou.xziqi.cn

Py:   except ValueError as e:
来源：http://kbl.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://thr.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://equ.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://dku.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ysr.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ite.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://rnp.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://slk.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://dgz.epnwcf.com

Py:   value = d.get("k") or default
来源：http://lmb.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rxj.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://dmw.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://lbd.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jxj.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yop.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://ssz.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://tgt.snrcjt.cn

[H07] 断言
来源：http://otg.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://kqb.shzxlz.cn

PHP:  assert($x > 0);
来源：http://czh.c1oappe.top

JS:   console.assert(x > 0);
来源：http://fob.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://drr.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://lsl.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sqf.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://edz.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://plg.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://irk.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://pvq.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yjw.zhengqikj.top

JS:   e.message;  e.stack
来源：http://blg.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://muj.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gwi.tian-w.cn

Go:   err.Error()
来源：http://puw.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://nmd.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://tvz.daxiang520.top

[H09] 带错误码的异常
来源：http://rco.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hgq.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://veb.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hpy.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mlx.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kkb.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydc.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://jxq.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lzz.pycfn.com

[H10] 资源自动释放
来源：http://ylp.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://suv.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyw.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xoy.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jgl.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://csr.epnwcf.com

Go:   defer f.Close()
来源：http://jod.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wzl.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nya.zhixingplan.top

================================================================================
来源：http://yuq.daxiang520.top

I. 正则表达式
来源：http://czg.sufxvd.cn

================================================================================
来源：http://ssb.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://efv.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xle.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://jew.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://ozx.hcnkem.com

TS:   /\d+/.test(s)
来源：http://uph.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gro.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yvz.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://ipo.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vfi.xinyue.icu

[I02] 提取所有匹配
来源：http://ydd.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://yrm.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fgf.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jhz.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://nzt.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rml.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pqr.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://ulk.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xla.guannengcc.top

[I03] 提取捕获分组
来源：http://jmq.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xcy.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jiz.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xzw.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nue.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ias.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vef.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ajb.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dlo.ivvv.top

[I04] 正则替换
来源：http://xnq.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nlf.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pjj.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ffb.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://saa.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bdc.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hfu.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://goo.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://coq.jianghu66.top

[I05] 按正则拆分
来源：http://ajb.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gtl.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rqa.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://dtv.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://buf.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://fdf.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aqh.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ydh.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vuf.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nbb.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jld.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jph.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krm.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fwk.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://feb.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bub.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pxt.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://khc.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://abz.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nln.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qiy.gotoacloud.top

TS:   /error/gim
来源：http://htw.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gra.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mgc.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://lgt.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wod.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://dnm.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pkb.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lmy.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vab.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvm.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lor.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tqa.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bsy.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ahj.fzhhl.top

================================================================================
来源：http://rmx.nanxuanxn.top

J. 日期与时间
来源：http://ywg.52xcode.cn

================================================================================
来源：http://fvh.hnxiangtu.top

[J01] 获取当前时间
来源：http://tzm.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lry.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rji.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://xvr.daxiang520.top

TS:   new Date();  Date.now()
来源：http://nsq.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oga.ehwqpu.com

Go:   time.Now()
来源：http://qne.shanyushiyangtech.top

Ruby: Time.now
来源：http://fgs.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pma.guannengcc.top

[J02] 格式化输出
来源：http://ppa.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yoc.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dry.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nev.hfpthk.cn

TS:   d.toISOString()
来源：http://ndc.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ycj.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dsd.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ays.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nsm.0kj1m.cn

[J03] 字符串解析为日期
来源：http://mvf.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://biv.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eur.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://iwl.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://woc.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://moi.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jjp.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://bzd.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ycx.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://ivx.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yrr.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iov.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://unb.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://zqj.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xkw.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://okn.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://erl.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wqw.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://qir.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://obe.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wik.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kna.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://swc.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://pmk.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://luf.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://hrn.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://rhi.zdqjudy.top

[J06] 计算两时间之差
来源：http://sjj.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://bcb.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://nuc.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jsy.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ygn.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://dbk.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://lcy.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://swd.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://wvf.fengsongda.top

[J07] 比较两个日期
来源：http://bcg.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://iiu.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qix.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pjs.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://vkw.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://thg.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://awj.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ugs.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://xzl.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://hga.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qcs.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jzz.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ael.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://arw.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rkn.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xbl.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qzt.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ecf.yuxming.cn

[J09] 时区处理
来源：http://ace.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://set.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nlf.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sid.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mkz.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bhr.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yau.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tzl.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yov.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://wpm.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pjg.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wdq.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pat.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uou.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xbi.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uso.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ums.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ajl.hcnkem.com

================================================================================
来源：http://enc.gotoacloud.top

K. JSON 与序列化
来源：http://smk.zhiwuduotai.top

================================================================================
来源：http://bgz.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://urw.hnqzz.top


<!-- 参考信息 -->