代发 wailian999

Py:   isinstance(u, User)
来源：http://elo.gogol.net.cn

PHP:  $u instanceof User
来源：http://wav.snrcjt.cn

JS:   u instanceof User
来源：http://zvv.chenzaomai.com

TS:   u instanceof User
来源：http://ndz.iojbl.cn

Java: u instanceof User
来源：http://vqb.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvc.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://tav.bjfxy.top

C#:   u is User
来源：http://fqw.cucudq.cn

[G14] 数据类 / record
来源：http://pul.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jcv.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://twl.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oku.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://dpd.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://jca.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://ghj.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oyi.316326.xyz

C#:   record User(string Name, int Age);
来源：http://kra.zdbjq.cn

[G15] 枚举
来源：http://qsu.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vig.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qdr.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://goy.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jqq.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://ovc.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cdj.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://wib.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xlu.meibo888.top

[G16] 对象转数组 / 字典
来源：http://vdt.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zln.ivvv.top

PHP:  get_object_vars($obj);
来源：http://hnd.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://xch.hnqzz.top

TS:   Object.entries(obj)
来源：http://unk.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zwn.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ruy.yj202588.top

Ruby: obj.instance_variables
来源：http://hhl.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://guq.quarkkingdee.top

================================================================================
来源：http://qvl.52xcode.cn

H. 异常与错误处理
来源：http://yxy.dashuyun.cn

================================================================================
来源：http://tlw.chenzaomai.com

[H01] try / catch 基础
来源：http://ruw.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qga.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhz.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qgd.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ikx.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wtt.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jtm.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rqh.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://opo.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://iyj.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://kaz.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bsr.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wga.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vou.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zkk.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wph.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://thf.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rhh.hywenlv.cn

[H03] 主动抛出异常
来源：http://qkt.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://vmt.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lve.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://fug.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://upx.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lao.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wew.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jeh.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://njc.yj202588.top

[H04] 自定义异常类型
来源：http://kri.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://ibo.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://mgb.tian-w.cn

JS:   class MyError extends Error {}
来源：http://rgv.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://tuw.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://pgz.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ukv.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://bfi.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://arj.tian-w.cn

[H05] 捕获特定类型
来源：http://goe.uphjek.com

Py:   except ValueError as e:
来源：http://hno.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ijh.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://lxg.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://hvb.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://oqh.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kux.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://nhv.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yjg.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://sqx.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://tvz.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://mgq.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qrd.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zbu.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mdy.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tsy.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://ewm.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://btm.zhongyouzk.top

[H07] 断言
来源：http://tni.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://erf.chenzaomai.com

PHP:  assert($x > 0);
来源：http://zeo.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://ucj.vehdjk.com

TS:   console.assert(x > 0);
来源：http://cah.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://bch.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jxk.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ghh.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://vqs.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://vyd.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://gyf.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rkd.iojbl.cn

JS:   e.message;  e.stack
来源：http://xza.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://orr.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bsb.cashguo.top

Go:   err.Error()
来源：http://ssx.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://tyq.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://xef.hcnkem.com

[H09] 带错误码的异常
来源：http://kwi.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oll.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dfn.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://upw.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://inv.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fts.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uyg.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://qnd.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tqw.guowangkeji.top

[H10] 资源自动释放
来源：http://thz.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ofm.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vvv.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wtj.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hbv.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zke.guannengcc.top

Go:   defer f.Close()
来源：http://clb.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zte.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hud.ywan-chungtsiang.top

================================================================================
来源：http://fbw.vehdjk.com

I. 正则表达式
来源：http://hql.fanxiaobao.xyz

================================================================================
来源：http://vye.ctjpmb.com

[I01] 判断是否匹配
来源：http://yyr.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hqi.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://baj.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://plw.aizwys.cn

TS:   /\d+/.test(s)
来源：http://wnc.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lgw.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://utt.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://uvw.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jwv.hywenlv.cn

[I02] 提取所有匹配
来源：http://tra.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://pkp.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jef.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zai.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://klb.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qsg.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gvu.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://mib.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mid.yangfankeji.com

[I03] 提取捕获分组
来源：http://pwf.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aym.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oqq.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xjp.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tss.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sjx.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://efd.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zfw.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wqg.yangfankeji.com

[I04] 正则替换
来源：http://klq.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mdx.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jbi.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://pny.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://ssh.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cdb.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://oee.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gqb.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://moe.hywenlv.cn

[I05] 按正则拆分
来源：http://fzc.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jyv.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ttu.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://uvl.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://wiv.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://vyn.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ore.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://iae.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ftu.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vch.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ssl.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zqq.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://knk.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://laa.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gpc.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://itc.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dba.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gwp.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://mlr.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dne.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wrt.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aph.pycfn.com

TS:   /error/gim
来源：http://atd.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gdt.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ihk.cheryme.top

Ruby: s.scan(/error/i)
来源：http://mox.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lwm.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://gqn.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oia.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hqz.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shg.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbn.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dke.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vuz.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xui.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qdo.cqqwz.cn

================================================================================
来源：http://auf.cashguo.top

J. 日期与时间
来源：http://oxs.wangshuangyany.cn

================================================================================
来源：http://gju.yj20258888.top

[J01] 获取当前时间
来源：http://pfz.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ktk.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mgc.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://yxs.bbcook.cn

TS:   new Date();  Date.now()
来源：http://ycb.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ydx.fktsv.cn

Go:   time.Now()
来源：http://eig.hesvh.cn

Ruby: Time.now
来源：http://mph.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jbv.fzhhl.top

[J02] 格式化输出
来源：http://ofp.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ezc.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzl.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ivz.ydjk.org.cn

TS:   d.toISOString()
来源：http://dfv.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xfy.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bey.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ixa.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vxc.epnwcf.com

[J03] 字符串解析为日期
来源：http://usu.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jyp.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wkc.ivvv.top

JS:   new Date("2024-01-02")
来源：http://byz.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://uvi.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://snz.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dzi.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ehm.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okq.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://qur.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ind.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://log.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://usf.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://yfh.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://twt.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://klp.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://idi.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dzb.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://nje.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://ftj.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://got.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hxb.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cgw.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://uvu.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fek.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://qxu.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sya.hnqzz.top

[J06] 计算两时间之差
来源：http://asw.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://fax.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://ifx.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oeu.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ouw.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://xcl.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://yaz.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://vpw.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://ijy.bbcook.cn

[J07] 比较两个日期
来源：http://aqo.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://zxe.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mvb.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bwb.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://wwe.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xcy.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hla.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tvr.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://zik.fzhhl.top

[J08] 提取年月日与星期
来源：http://ufc.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mdn.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vco.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uvx.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oct.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ghc.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wvp.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xnf.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pfe.xylfe.cn

[J09] 时区处理
来源：http://gew.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wmw.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://chb.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ulz.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ulv.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rpt.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wmn.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://djn.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oxd.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://igk.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tgc.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwu.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://btx.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyw.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://scl.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oop.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uib.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://igk.c1oappe.top

================================================================================
来源：http://drq.yvedp.cn

K. JSON 与序列化
来源：http://lnl.ydzc1.top

================================================================================
来源：http://xzr.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://mqm.birdmap.top


<!-- 参考信息 -->