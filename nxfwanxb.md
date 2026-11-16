代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://zqv.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://rox.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://hyu.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://iqd.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://urh.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://ptg.havefunace.top

C#:   public override string ToString() => Name;
来源：http://unl.hysaishi.cn

[G13] 判断对象类型
来源：http://nmr.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://tos.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://zrq.zhengqikj.top

JS:   u instanceof User
来源：http://jza.guowangkeji.top

TS:   u instanceof User
来源：http://ull.zhijiandao.cn

Java: u instanceof User
来源：http://ygl.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iap.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://tnt.fanxiaobao.xyz

C#:   u is User
来源：http://urf.hfpthk.cn

[G14] 数据类 / record
来源：http://ntv.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sbb.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://dsx.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://zhk.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://nrb.jianghu66.top

Java: record User(String name, int age) {}
来源：http://rlf.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://wtn.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://osg.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://cwz.xuanzx.com

[G15] 枚举
来源：http://yii.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hcv.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nkl.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hsb.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vzr.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://yoo.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ctx.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://uoc.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iuz.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://hac.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wlo.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://wfj.xuanzx.com

JS:   Object.entries(obj)
来源：http://bei.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://dmq.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eee.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gak.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://mxo.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://yzx.jqgfzy.top

================================================================================
来源：http://ume.yueranfly.top

H. 异常与错误处理
来源：http://cxu.vehdjk.com

================================================================================
来源：http://afg.bjfxy.top

[H01] try / catch 基础
来源：http://zrd.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nhl.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://phq.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kua.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qis.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yqc.iojbl.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qwr.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sfi.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oiy.fzhhl.top

[H02] finally / ensure 收尾
来源：http://bhf.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sca.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hjm.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://asl.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bqw.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ndr.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cwd.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uon.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cdn.zdqjudy.top

[H03] 主动抛出异常
来源：http://qrc.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://xpy.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dxg.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://kho.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://kxp.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uva.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyw.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sks.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zul.guowangkeji.top

[H04] 自定义异常类型
来源：http://gzm.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://qwc.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://dvj.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://kkm.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://ppv.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://qdv.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://spn.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://vrj.cucudq.cn

C#:   class MyException : Exception {}
来源：http://mry.mhx1999.top

[H05] 捕获特定类型
来源：http://isp.chenlongwang.top

Py:   except ValueError as e:
来源：http://vgw.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ktw.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://its.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://diy.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://upz.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nhg.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://fzk.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eov.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://vct.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://egz.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://rdd.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://smc.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://xjq.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xtx.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xhw.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://bkk.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://hsi.kuanghao11.cn

[H07] 断言
来源：http://ilc.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://vaw.dianchejie.cn

PHP:  assert($x > 0);
来源：http://ngf.gzhubu.top

JS:   console.assert(x > 0);
来源：http://bxp.sysykeji.top

TS:   console.assert(x > 0);
来源：http://vju.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://mzn.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fwt.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kmn.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://zkx.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://jil.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://fkt.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lcj.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://rnw.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bnm.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://abp.jianghu66.top

Go:   err.Error()
来源：http://ykh.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://gvs.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://rwp.zhongyouzk.top

[H09] 带错误码的异常
来源：http://gsg.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lwt.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kqc.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qsv.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cbu.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ejk.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://csl.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://dpt.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nph.fehbvm.com

[H10] 资源自动释放
来源：http://vlh.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pyb.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyj.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ndr.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ciz.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wni.ivvv.top

Go:   defer f.Close()
来源：http://guf.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kcp.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gkd.vqdsnc.cn

================================================================================
来源：http://vdm.zhaomingkeji.xyz

I. 正则表达式
来源：http://kdc.snrcjt.cn

================================================================================
来源：http://aay.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://uvz.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uex.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tui.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://oql.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://qlm.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rqm.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lrb.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://zrj.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xkq.gogol.net.cn

[I02] 提取所有匹配
来源：http://bnk.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://dih.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yhe.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asw.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://gpz.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xxd.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hcy.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://kdx.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kxk.andypj.xyz

[I03] 提取捕获分组
来源：http://kar.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zbi.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqf.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cne.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gau.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://btw.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bhp.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fkr.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rwl.zdbjq.cn

[I04] 正则替换
来源：http://ubi.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qxg.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gyf.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://whe.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://tmw.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://lfc.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://aur.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yen.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hap.zhoulong.xyz

[I05] 按正则拆分
来源：http://uan.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ydl.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lza.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://rly.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://ndk.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://sga.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://snq.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uod.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cti.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ran.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ude.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lno.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ipx.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clg.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yeu.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sxe.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ptj.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sdz.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://njn.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gsg.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nsq.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bke.mhx1999.top

TS:   /error/gim
来源：http://vii.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jza.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pxn.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://hcd.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oot.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://hdn.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iyt.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wmt.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ggs.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzz.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://myc.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://orf.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://csx.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qma.shzxlz.cn

================================================================================
来源：http://fxn.dashuyun.cn

J. 日期与时间
来源：http://bgg.316326.xyz

================================================================================
来源：http://jxx.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://qdi.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://seb.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehb.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://vvw.zycfv.cn

TS:   new Date();  Date.now()
来源：http://qcb.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://abu.bjfxy.top

Go:   time.Now()
来源：http://qxk.hywenlv.cn

Ruby: Time.now
来源：http://stx.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vyq.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://dqp.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ini.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zxx.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zuf.shzxlz.cn

TS:   d.toISOString()
来源：http://gea.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gti.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://afb.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhe.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ouj.daria6918.cn

[J03] 字符串解析为日期
来源：http://hvr.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eqn.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rjv.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://dox.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://uyw.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://apf.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aui.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://haz.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yic.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://nfl.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hmw.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://liq.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rub.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rxm.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fci.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uwv.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dlj.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jfm.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://wdr.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://urq.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ege.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zul.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nwh.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://zct.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qqb.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://tzd.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tgm.guowangkeji.top

[J06] 计算两时间之差
来源：http://sii.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://gdq.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://vmk.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svr.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sam.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://vrf.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://zul.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://nit.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://cmt.jqgfzy.top

[J07] 比较两个日期
来源：http://qnc.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://nqx.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vpn.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://jyq.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nue.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atd.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lrx.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bks.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://hxp.cqqwz.cn

[J08] 提取年月日与星期
来源：http://fuq.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://imw.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wge.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wpc.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eob.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://owz.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zzc.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ejx.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rck.jinyuanbaomall.cn

[J09] 时区处理
来源：http://gql.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xhk.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pyn.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywu.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oxa.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eel.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://phz.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://usc.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vji.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://fca.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yec.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://loo.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qfj.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lpv.sysykeji.top


<!-- 参考信息 -->