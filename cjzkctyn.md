代发 wailian999

[G14] 数据类 / record
来源：http://kbn.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zhk.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://kgz.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://sdq.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://ckj.yueranfly.top

Java: record User(String name, int age) {}
来源：http://zfg.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://fnh.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vuj.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://lxo.cucudq.cn

[G15] 枚举
来源：http://kvs.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vhc.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ddv.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjl.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tpq.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://zrd.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rlp.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://nse.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rjp.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://czf.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbc.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://zmq.vehdjk.com

JS:   Object.entries(obj)
来源：http://xjg.cqqwz.cn

TS:   Object.entries(obj)
来源：http://sqr.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rog.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cen.sxryk.cn

Ruby: obj.instance_variables
来源：http://ptp.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://osb.yongpay.top

================================================================================
来源：http://sdn.jqgfzy.top

H. 异常与错误处理
来源：http://ojo.wangshuangyany.cn

================================================================================
来源：http://ltw.zhijiandao.cn

[H01] try / catch 基础
来源：http://xsd.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wzl.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fij.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nem.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gza.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://scw.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cdg.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qee.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bhp.zhixingplan.top

[H02] finally / ensure 收尾
来源：http://gtg.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ebv.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hcu.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vjv.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gou.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://huc.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vbs.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pxv.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rac.nanxinkj.top

[H03] 主动抛出异常
来源：http://fmh.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://iym.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ijq.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://aub.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://svb.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://snh.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lxg.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mvh.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rrs.zdbjq.cn

[H04] 自定义异常类型
来源：http://ulw.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://vds.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jbe.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://odx.yueranfly.top

TS:   class MyError extends Error {}
来源：http://mem.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://lwc.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xnf.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://qnz.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://mjn.xinyue.icu

[H05] 捕获特定类型
来源：http://kut.epnwcf.com

Py:   except ValueError as e:
来源：http://unw.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ovx.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://dew.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://zqi.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://fbt.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lvt.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://mxg.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://srl.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://kwl.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://nxm.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zyo.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://orf.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ymz.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://efb.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vkz.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://whu.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://fdl.sxryk.cn

[H07] 断言
来源：http://xmb.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://xbh.yonumen.top

PHP:  assert($x > 0);
来源：http://xms.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://mik.andypj.xyz

TS:   console.assert(x > 0);
来源：http://lyt.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://bgh.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fta.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://ksi.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://zus.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://mjp.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://dxz.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hfs.xziqi.cn

JS:   e.message;  e.stack
来源：http://cea.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://our.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ywu.hammf.cn

Go:   err.Error()
来源：http://xzj.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://byc.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://dcp.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://oaf.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mep.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwp.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uum.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytx.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qyc.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vbi.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fwu.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qea.yuanzhike.top

[H10] 资源自动释放
来源：http://ysw.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyl.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yyr.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://don.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hhg.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nds.tarul.cn

Go:   defer f.Close()
来源：http://rfd.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ubl.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xct.nanxuanxn.top

================================================================================
来源：http://bhj.mhx1999.top

I. 正则表达式
来源：http://fky.jinqigufen.top

================================================================================
来源：http://iha.sjlbkw.cn

[I01] 判断是否匹配
来源：http://qwb.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nco.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://edk.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://oqx.guannengcc.top

TS:   /\d+/.test(s)
来源：http://dqi.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lup.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ncc.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://iph.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dtf.9152youxi.cn

[I02] 提取所有匹配
来源：http://foj.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://wgq.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bvv.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dxn.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://qtu.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jne.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://odb.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://okx.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xqx.jianghu66.top

[I03] 提取捕获分组
来源：http://woo.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jrj.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qid.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qel.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ysi.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wfe.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gpn.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dvn.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eyb.ehwqpu.com

[I04] 正则替换
来源：http://uqo.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eao.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ckf.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://owe.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eqk.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://cwo.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://los.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rsa.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://too.jianghu66.top

[I05] 按正则拆分
来源：http://swo.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mzu.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lcj.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://opf.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://jon.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://eps.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lii.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fpx.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dlt.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qdq.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dsn.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://erq.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gmm.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sli.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wsr.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nvd.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jzv.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qgr.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://pgq.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lap.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ihz.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oog.0kj1m.cn

TS:   /error/gim
来源：http://rjf.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pyy.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://buq.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://vrj.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzu.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://odq.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yjw.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://psy.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xyz.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wya.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dpu.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://shm.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://drj.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://epf.shzxlz.cn

================================================================================
来源：http://wdy.gzhubu.top

J. 日期与时间
来源：http://art.zhiwuduotai.top

================================================================================
来源：http://bwc.gzhubu.top

[J01] 获取当前时间
来源：http://sxx.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hoq.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pcd.fengsongda.top

JS:   new Date();  Date.now()
来源：http://vwq.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://rck.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://shh.tarul.cn

Go:   time.Now()
来源：http://lzs.feifeiyinyue.top

Ruby: Time.now
来源：http://ayt.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qct.daria6918.cn

[J02] 格式化输出
来源：http://lvm.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zib.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pfa.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lzv.jqgfzy.top

TS:   d.toISOString()
来源：http://mik.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmi.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zig.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iyi.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tkb.9152youxi.cn

[J03] 字符串解析为日期
来源：http://czy.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uqv.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xhd.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://ucf.tanke756.top

TS:   new Date("2024-01-02")
来源：http://zal.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://rua.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lpe.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://glq.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fof.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://ava.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jck.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kyf.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pop.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kyx.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dmp.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iyq.sufxvd.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uoc.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ywx.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://gon.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ssa.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://etk.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hky.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vge.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://jmz.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://avt.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://tvg.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://zlw.shuidangran.top

[J06] 计算两时间之差
来源：http://pat.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://zrt.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://gsx.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zop.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bqf.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qwj.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://dxj.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://ant.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://and.jqgufenzy.top

[J07] 比较两个日期
来源：http://yqs.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://xat.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sex.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://oqr.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://qua.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbr.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rmn.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://zxd.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://vvh.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://lai.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyk.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mgl.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uty.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://taa.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pna.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oes.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mai.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pht.cqqwz.cn

[J09] 时区处理
来源：http://qax.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://prx.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tgq.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iih.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnp.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bsv.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pkq.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://kht.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://syi.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://lhy.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zlm.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fba.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iyw.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jdv.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dim.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emc.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tki.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://skk.andypj.xyz

================================================================================
来源：http://xvt.fehbvm.com

K. JSON 与序列化
来源：http://bjg.hcnkem.com

================================================================================
来源：http://obb.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://kur.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tix.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wpr.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://jee.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://ost.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nal.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://rad.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hvx.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://udw.kuanghao11.cn


<!-- 参考信息 -->