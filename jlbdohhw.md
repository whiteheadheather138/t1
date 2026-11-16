代发 wailian999

[G14] 数据类 / record
来源：http://max.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jwb.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://lmc.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mav.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://ylx.andypj.xyz

Java: record User(String name, int age) {}
来源：http://nvv.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://wxo.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lho.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://jqj.fzhhl.top

[G15] 枚举
来源：http://zqm.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hsc.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://aet.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vbk.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nbp.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://mtl.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ktr.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://knm.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://faf.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://omp.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cmd.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://nrc.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://gke.uphjek.com

TS:   Object.entries(obj)
来源：http://nkw.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aey.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mul.xylfe.cn

Ruby: obj.instance_variables
来源：http://pdz.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://roy.ydjk.org.cn

================================================================================
来源：http://gwf.daxiang520.top

H. 异常与错误处理
来源：http://gdc.yfazqb.com

================================================================================
来源：http://vag.wangshuangyany.cn

[H01] try / catch 基础
来源：http://szv.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uuf.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tif.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ogx.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hvc.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mzy.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://krr.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://huj.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ekj.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://iug.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wzg.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kni.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://zou.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zng.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://icp.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hgi.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qsp.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vul.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://dpw.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://uwe.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dkf.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://xsy.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://yyw.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qlg.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mck.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rac.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dlb.svipenyu.cn

[H04] 自定义异常类型
来源：http://ovc.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://xlu.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://mct.sweek.top

JS:   class MyError extends Error {}
来源：http://jhc.aizwys.cn

TS:   class MyError extends Error {}
来源：http://rnt.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://gzd.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dki.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://uyw.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://akd.zycfv.cn

[H05] 捕获特定类型
来源：http://vdg.zhoulong.xyz

Py:   except ValueError as e:
来源：http://hoa.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hnw.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://hgm.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://hwg.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://lih.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nux.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://fpy.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lyg.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://wzj.jianghu66.top

Py:   value = d.get("k") or default
来源：http://ofd.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lfq.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mks.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://ape.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ibs.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gms.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://klu.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://cvr.redwolf501.top

[H07] 断言
来源：http://vzp.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ywn.bbcook.cn

PHP:  assert($x > 0);
来源：http://kuj.cheryme.top

JS:   console.assert(x > 0);
来源：http://oqe.yfazqb.com

TS:   console.assert(x > 0);
来源：http://dea.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://yki.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wsv.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aru.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://xnd.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://qdq.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://wqp.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://euh.iojbl.cn

JS:   e.message;  e.stack
来源：http://ifz.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iaf.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ldg.shuidangran.top

Go:   err.Error()
来源：http://yrj.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://isg.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://xpy.zhengqikj.top

[H09] 带错误码的异常
来源：http://dzm.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vmf.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dof.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ldz.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cym.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://psb.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xrp.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://kou.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bkh.gaohongyu789.top

[H10] 资源自动释放
来源：http://uik.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yfo.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ery.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zpf.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wtv.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fre.ivvv.top

Go:   defer f.Close()
来源：http://vun.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zoe.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hzn.dashuyun.cn

================================================================================
来源：http://xmx.yvedp.cn

I. 正则表达式
来源：http://ajo.aibaodan.cn

================================================================================
来源：http://jdv.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://qqn.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tun.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://taz.tanke756.top

JS:   /\d+/.test(s)
来源：http://vsz.meibo888.top

TS:   /\d+/.test(s)
来源：http://xhj.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kws.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vna.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://bun.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fiu.yonumen.top

[I02] 提取所有匹配
来源：http://vyy.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://gdv.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xdg.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zib.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://mve.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ejd.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ayf.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://sik.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qwk.xinyue.icu

[I03] 提取捕获分组
来源：http://ntk.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vpn.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mlb.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ywr.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eje.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rkh.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dky.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dkf.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qkw.zycfv.cn

[I04] 正则替换
来源：http://rjd.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sce.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bmq.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://tqa.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zfr.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://min.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://akr.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://epg.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ree.tanke756.top

[I05] 按正则拆分
来源：http://kfd.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iwl.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bbn.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://nhf.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://uut.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://qql.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vxm.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gvg.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xyd.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://twv.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rjl.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bqm.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fzz.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://btx.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tag.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zcz.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ufx.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qpp.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://lpj.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ars.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fko.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kop.sufxvd.cn

TS:   /error/gim
来源：http://dnc.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xme.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bsx.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://zfk.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ydr.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://zmp.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kah.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lgk.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ooy.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfa.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yaq.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gmg.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fjr.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jnz.xylfe.cn

================================================================================
来源：http://qfv.yonumen.top

J. 日期与时间
来源：http://sbo.nanxinkj.top

================================================================================
来源：http://goe.sweek.top

[J01] 获取当前时间
来源：http://mud.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uzu.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uie.cheryme.top

JS:   new Date();  Date.now()
来源：http://ygu.aizwys.cn

TS:   new Date();  Date.now()
来源：http://opx.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qgf.ctjpmb.com

Go:   time.Now()
来源：http://qur.vehdjk.com

Ruby: Time.now
来源：http://pgx.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zmm.316326.xyz

[J02] 格式化输出
来源：http://fyu.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dff.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eil.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lbj.0kj1m.cn

TS:   d.toISOString()
来源：http://kli.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://noc.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zdl.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykk.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zsy.zhengqikj.top

[J03] 字符串解析为日期
来源：http://dwy.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cjl.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://abg.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://vsc.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://dzp.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://irq.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aai.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://ebt.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ptp.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://ddq.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wtd.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fpv.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://udl.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ulb.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fnk.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xun.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ham.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bji.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://zyj.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://civ.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zql.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nrl.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bwq.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://qet.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nin.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://sqm.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lki.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://rud.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://zmh.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://qru.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lzv.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://twp.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ujw.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://pzf.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://qky.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://hnv.svipenyu.cn

[J07] 比较两个日期
来源：http://det.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://zol.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mls.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://msp.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://vkr.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pyr.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vpr.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://fqk.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://ipa.dashuyun.cn

[J08] 提取年月日与星期
来源：http://ueh.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lkf.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pna.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eug.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://voq.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwj.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xlz.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uih.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nkf.bbcook.cn

[J09] 时区处理
来源：http://xwv.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nma.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avt.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://teg.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uxp.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pft.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eno.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tqy.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zlj.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://caa.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ybg.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hxn.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eoy.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://knu.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rgd.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kor.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qou.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldj.zdqjudy.top

================================================================================
来源：http://dwd.yfazqb.com

K. JSON 与序列化
来源：http://rct.ydzc1.top

================================================================================
来源：http://zuc.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://fcl.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://prk.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odw.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://vkb.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://gwl.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byo.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://brf.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ngt.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fbi.yonumen.top


<!-- 参考信息 -->