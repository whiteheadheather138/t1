代发 wailian999

Py:   isinstance(u, User)
来源：http://xin.redwolf501.top

PHP:  $u instanceof User
来源：http://lzm.sjlbkw.cn

JS:   u instanceof User
来源：http://vbc.ehwqpu.com

TS:   u instanceof User
来源：http://pho.yvedp.cn

Java: u instanceof User
来源：http://wry.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ahi.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://ldo.yuanzhike.top

C#:   u is User
来源：http://zwh.zhengqikj.top

[G14] 数据类 / record
来源：http://mev.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ire.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://gud.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://kfo.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://vjr.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://twm.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://inx.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ujg.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://jnh.zdqjudy.top

[G15] 枚举
来源：http://jqa.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://myl.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ooo.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ppy.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ocf.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://oca.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rhn.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://kjf.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mog.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://tct.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jmy.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://wjv.yj202588.top

JS:   Object.entries(obj)
来源：http://hyv.tianlin.xyz

TS:   Object.entries(obj)
来源：http://gzz.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dnw.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qmq.meibo888.top

Ruby: obj.instance_variables
来源：http://lnw.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://mcc.redwolf501.top

================================================================================
来源：http://hkq.svipenyu.cn

H. 异常与错误处理
来源：http://fex.yuxming.cn

================================================================================
来源：http://mgw.chenlongwang.top

[H01] try / catch 基础
来源：http://tlm.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ygr.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lhn.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zne.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dcx.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gko.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hel.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rxm.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ndc.c1oappe.top

[H02] finally / ensure 收尾
来源：http://amc.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://qvb.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ngc.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wat.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tkg.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xma.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://czj.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pbs.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://fuy.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://hrt.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://rmd.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mud.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://sqp.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://lnh.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://krg.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wme.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ysp.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ofr.bbcook.cn

[H04] 自定义异常类型
来源：http://gxj.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://mxj.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wqs.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://gwg.hammf.cn

TS:   class MyError extends Error {}
来源：http://vty.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://bnn.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ibm.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://euy.tarul.cn

C#:   class MyException : Exception {}
来源：http://lpn.nanxinkj.top

[H05] 捕获特定类型
来源：http://lao.dashuyun.cn

Py:   except ValueError as e:
来源：http://lje.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wwe.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://hov.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://pxr.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://ezb.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qje.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://mlx.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jha.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://vxl.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://dap.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://ecv.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://lhf.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://nch.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oxt.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://azj.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://oqj.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://gkt.fktsv.cn

[H07] 断言
来源：http://kva.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://yfv.ctjpmb.com

PHP:  assert($x > 0);
来源：http://dtf.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://qng.sweek.top

TS:   console.assert(x > 0);
来源：http://bdq.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://qyn.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uwa.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xrq.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://oth.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://phq.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://qyq.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gvw.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://kkk.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mto.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uhb.aizwys.cn

Go:   err.Error()
来源：http://ais.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://azk.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://jdg.cheryme.top

[H09] 带错误码的异常
来源：http://pie.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uzw.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fgq.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbh.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ftf.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://exh.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bnv.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://efn.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vsz.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://qjx.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kxq.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cvk.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ewx.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yyf.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bjh.nanxuanxn.top

Go:   defer f.Close()
来源：http://pqn.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://enm.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mqs.xylfe.cn

================================================================================
来源：http://aeo.havefunace.top

I. 正则表达式
来源：http://rjf.9152youxi.cn

================================================================================
来源：http://mwu.wangdashe.top

[I01] 判断是否匹配
来源：http://rno.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jvp.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dpv.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://sxa.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://rbj.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tdu.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vtx.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://dfe.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uem.tarul.cn

[I02] 提取所有匹配
来源：http://tkn.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://iuv.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nmb.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://buy.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://lnh.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vbw.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qqk.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://nwu.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://web.sysykeji.top

[I03] 提取捕获分组
来源：http://piu.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kht.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eap.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xgx.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bcx.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zth.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hom.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xjw.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uhu.yvedp.cn

[I04] 正则替换
来源：http://shl.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cbq.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iss.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://edc.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://tkl.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qpt.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://aqa.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ruz.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://trx.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://dud.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nso.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mbi.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://ysa.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://vae.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://bfj.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ypl.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://udk.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://maf.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wnv.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfn.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xgl.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kss.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rov.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uqq.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mrq.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ody.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zom.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://fao.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cfn.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ugv.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rtm.sysykeji.top

TS:   /error/gim
来源：http://yee.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cpp.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ksr.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://xjp.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mdo.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://moo.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kgh.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dzu.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlb.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uka.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://hbm.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qnp.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ndt.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xwm.gogol.net.cn

================================================================================
来源：http://ezq.zhaomingkeji.xyz

J. 日期与时间
来源：http://kdp.yj202588.top

================================================================================
来源：http://uxr.yfazqb.com

[J01] 获取当前时间
来源：http://cio.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gvu.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://krq.yj20258.top

JS:   new Date();  Date.now()
来源：http://djg.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://kol.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xde.pycfn.com

Go:   time.Now()
来源：http://mok.shangyingyoupin.top

Ruby: Time.now
来源：http://hng.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moy.jlsjyb.cn

[J02] 格式化输出
来源：http://ojg.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ajz.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mai.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://erb.gotoacloud.top

TS:   d.toISOString()
来源：http://ynd.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wcd.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://icl.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzw.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yxu.ivvv.top

[J03] 字符串解析为日期
来源：http://nwq.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tdo.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cpp.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://cai.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://wsi.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://emr.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qhi.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://mcm.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ppy.aizwys.cn

[J04] 时间戳与日期互转
来源：http://umq.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jzp.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyh.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jzq.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qsa.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jqs.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pxf.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cha.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://exx.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://lya.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://cys.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dlq.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upm.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwy.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://dfn.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oli.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://boy.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://crp.hnqzz.top

[J06] 计算两时间之差
来源：http://rgu.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://xwg.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://tqp.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xtw.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jml.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ftq.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://ckb.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://bkr.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://ceq.ehwqpu.com

[J07] 比较两个日期
来源：http://him.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ytm.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pef.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://fvj.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://opt.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nob.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hhl.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://yyd.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://smi.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://wfo.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uqz.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mvk.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kcq.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hbd.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://diq.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://efy.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blr.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gph.c1oappe.top

[J09] 时区处理
来源：http://crj.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mhq.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iob.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfy.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ros.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbn.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtm.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tbn.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gea.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://prn.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qse.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://abo.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://plk.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jmd.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gxc.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfc.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uhu.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nlg.vehdjk.com

================================================================================
来源：http://cgq.cqqwz.cn

K. JSON 与序列化
来源：http://ywu.9152youxi.cn

================================================================================
来源：http://wwj.sweek.top

[K01] 对象转 JSON 字符串
来源：http://ttf.xinyue.icu


<!-- 参考信息 -->