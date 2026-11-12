代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://tna.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://gfg.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://eos.sweek.top

Java: @Override public String toString() { return name; }
来源：http://tob.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nqr.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://vum.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://vdq.feifeiyinyue.top

[G13] 判断对象类型
来源：http://qch.dianchejie.cn

Py:   isinstance(u, User)
来源：http://mhu.tarul.cn

PHP:  $u instanceof User
来源：http://wkq.cucudq.cn

JS:   u instanceof User
来源：http://ljm.hammf.cn

TS:   u instanceof User
来源：http://aky.xziqi.cn

Java: u instanceof User
来源：http://vkr.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hfu.c1oappe.top

Ruby: u.is_a?(User)
来源：http://fxn.cheryme.top

C#:   u is User
来源：http://pth.guowangkeji.top

[G14] 数据类 / record
来源：http://cer.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ckh.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://koz.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://maq.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://ouf.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://yyu.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://ura.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grz.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://rtf.feifeiyinyue.top

[G15] 枚举
来源：http://kwr.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qiw.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://thn.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lco.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wpf.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://yai.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ejb.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://hxo.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ize.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://zly.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ktr.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://tmi.shuidangran.top

JS:   Object.entries(obj)
来源：http://kde.haohaochexian.top

TS:   Object.entries(obj)
来源：http://mcf.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wnc.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://joj.hnqzz.top

Ruby: obj.instance_variables
来源：http://qkd.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://xda.feifeiyinyue.top

================================================================================
来源：http://wzr.chenlongwang.top

H. 异常与错误处理
来源：http://qei.hywenlv.cn

================================================================================
来源：http://dml.xuetiantiany.cn

[H01] try / catch 基础
来源：http://ekk.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://htq.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://exb.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lzn.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jco.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vha.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wvb.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fht.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tsd.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://cgm.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxg.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mdb.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nmv.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yji.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ejw.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fxr.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fef.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wtn.hywenlv.cn

[H03] 主动抛出异常
来源：http://iwx.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://bfq.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hyx.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://tir.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://pdu.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gax.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rzt.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ari.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://hhw.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://elj.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://oos.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://dqu.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://jjw.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://bir.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://ioo.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nch.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://png.redwolf501.top

C#:   class MyException : Exception {}
来源：http://mfo.zycfv.cn

[H05] 捕获特定类型
来源：http://kal.jinqigfzy.top

Py:   except ValueError as e:
来源：http://vbk.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xqo.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://rsw.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://abf.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://xak.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rwd.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://jbr.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rkf.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://tgd.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://ntf.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://iuk.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://qcc.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://inx.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bsf.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kca.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://scl.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://lms.ivvv.top

[H07] 断言
来源：http://xfh.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://kfv.sufxvd.cn

PHP:  assert($x > 0);
来源：http://amw.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://gtv.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://lyz.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://fnn.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uuk.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://cuv.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://gnp.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://yur.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://edf.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://plu.bjfxy.top

JS:   e.message;  e.stack
来源：http://mxs.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vhf.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dom.tian-w.cn

Go:   err.Error()
来源：http://vhf.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://xsx.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://zvp.jiagoushi.top

[H09] 带错误码的异常
来源：http://rhz.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mph.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hxt.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yiw.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jiu.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ukc.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://poq.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://acq.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ouh.tianlin.xyz

[H10] 资源自动释放
来源：http://ahb.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dbz.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dya.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://obl.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://otp.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ibg.snrcjt.cn

Go:   defer f.Close()
来源：http://lug.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tld.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fvh.jinqigufen.top

================================================================================
来源：http://hwo.pengpengdd.cyou

I. 正则表达式
来源：http://owb.ppjwa.cn

================================================================================
来源：http://amu.zhengqikj.top

[I01] 判断是否匹配
来源：http://ujy.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fpj.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bpp.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://del.yj20258888.top

TS:   /\d+/.test(s)
来源：http://dxa.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xbi.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qvk.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://bbv.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qgm.hnqzz.top

[I02] 提取所有匹配
来源：http://aie.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://jvk.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rpy.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fby.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://ece.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://grj.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://njd.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://cbo.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lgy.yuxming.cn

[I03] 提取捕获分组
来源：http://cjj.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pth.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tap.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://asg.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rgo.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tgl.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://etd.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvh.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hea.svipenyu.cn

[I04] 正则替换
来源：http://fdg.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lxu.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://php.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hpj.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://vdy.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://eww.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://upg.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pab.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bnq.sjlbkw.cn

[I05] 按正则拆分
来源：http://wxr.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://seq.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gur.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://xku.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://kob.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://aef.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dpc.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wkd.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lkg.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://glq.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bwo.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://npt.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpj.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmk.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ukg.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fgu.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bmh.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txu.sweek.top

[I07] 忽略大小写与多行模式
来源：http://ljc.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://syg.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kko.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://slg.zhijiandao.cn

TS:   /error/gim
来源：http://pyl.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://whc.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://olk.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://hok.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://veg.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://hug.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xul.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yqr.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmw.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uyp.guannengcc.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rwp.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bfm.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uvv.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wva.jinqigufen.top

================================================================================
来源：http://xfu.hongshengwenyu.top

J. 日期与时间
来源：http://rcz.jqgufenzy.top

================================================================================
来源：http://vsy.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://npi.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://plc.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gom.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://gjk.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://fxv.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oir.jinqigfzy.top

Go:   time.Now()
来源：http://fmn.fzhhl.top

Ruby: Time.now
来源：http://jbx.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fpy.ydzc1.top

[J02] 格式化输出
来源：http://cms.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebe.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mwe.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tli.cashguo.top

TS:   d.toISOString()
来源：http://mnp.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://smf.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hvn.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ays.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kap.havefunace.top

[J03] 字符串解析为日期
来源：http://vww.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cgc.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://osd.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://zjh.pycfn.com

TS:   new Date("2024-01-02")
来源：http://cyl.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bbv.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zgh.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://omr.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nsx.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://twg.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hpn.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccf.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ezs.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hbd.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qih.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vee.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bie.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://poz.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://luf.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://erj.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oin.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vag.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ley.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://sqa.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qwf.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://iwe.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://sra.pycfn.com

[J06] 计算两时间之差
来源：http://agl.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://zms.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://ily.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mqi.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mdd.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://nrn.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://fak.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://ktj.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://qpa.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://kgy.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://rfr.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hfl.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://idb.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://tvi.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fni.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bjc.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yrt.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://hxq.0kj1m.cn

[J08] 提取年月日与星期
来源：http://zud.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hoi.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iqn.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xve.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zei.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ibz.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://udh.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hsx.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rfk.chenzaomai.com

[J09] 时区处理
来源：http://wtg.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qtb.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qht.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rrf.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxf.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dfi.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cko.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pvt.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jaj.sweek.top

[J10] 取今天 / 本月第一天
来源：http://wpy.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://khn.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://acq.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bde.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vcy.yangfankeji.com


<!-- 参考信息 -->