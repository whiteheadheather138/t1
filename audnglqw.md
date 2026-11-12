代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://nqx.fzhhl.top

JS:   toString() { return this.name; }
来源：http://oat.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://xpj.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://rpc.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://zzq.guannengcc.top

Ruby: def to_s; @name; end
来源：http://vzz.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://zgc.epnwcf.com

[G13] 判断对象类型
来源：http://otk.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://ghs.epnwcf.com

PHP:  $u instanceof User
来源：http://wag.c1oappe.top

JS:   u instanceof User
来源：http://yag.yueranfly.top

TS:   u instanceof User
来源：http://eih.ywan-chungtsiang.top

Java: u instanceof User
来源：http://eol.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wsc.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://fgq.yj20258.top

C#:   u is User
来源：http://yvw.ybcxt.top

[G14] 数据类 / record
来源：http://duk.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xkt.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://oyx.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qzb.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://pja.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://rui.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://iet.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://huj.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://lpp.shanyushiyangtech.top

[G15] 枚举
来源：http://ltm.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wxt.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ahz.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://syh.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eae.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://cmj.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uxp.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://ljy.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ihh.yj20258.top

[G16] 对象转数组 / 字典
来源：http://wrh.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rda.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://ecs.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://tzj.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://eyq.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jmk.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jlo.hnqzz.top

Ruby: obj.instance_variables
来源：http://glt.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://job.zhiwuduotai.top

================================================================================
来源：http://nxb.zhijiandao.cn

H. 异常与错误处理
来源：http://ntx.meibo888.top

================================================================================
来源：http://fnz.0kj1m.cn

[H01] try / catch 基础
来源：http://nce.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ufo.dianchejie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rgj.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rmg.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://siu.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lmy.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yeg.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xxd.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ikn.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://iou.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://fes.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qow.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sna.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wqt.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://opy.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tlx.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lqg.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lka.sxryk.cn

[H03] 主动抛出异常
来源：http://cnw.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://mvh.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uye.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://ada.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://unv.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tcz.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aip.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kba.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://iry.tanke756.top

[H04] 自定义异常类型
来源：http://olg.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://gpf.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qcx.ivvv.top

JS:   class MyError extends Error {}
来源：http://inz.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://zsw.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://vkl.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://any.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://hqy.yj20258888.top

C#:   class MyException : Exception {}
来源：http://aiu.gzhubu.top

[H05] 捕获特定类型
来源：http://ngo.wangdashe.top

Py:   except ValueError as e:
来源：http://jpw.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ujq.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://qjl.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://hrn.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://dnz.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lma.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://wgk.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qtl.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://tjn.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://yxe.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://yro.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://cvh.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://udw.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://shq.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qty.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://mfx.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://wha.jqgufenzy.top

[H07] 断言
来源：http://qff.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://kcg.xylfe.cn

PHP:  assert($x > 0);
来源：http://qym.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://aqw.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://sql.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://rxg.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gyj.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://odd.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://tiy.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://rhn.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://lwr.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jre.ydzc1.top

JS:   e.message;  e.stack
来源：http://lwm.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rsx.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://uip.jianghu66.top

Go:   err.Error()
来源：http://prk.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://mfa.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://tce.hnqzz.top

[H09] 带错误码的异常
来源：http://jku.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yte.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ods.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hrg.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xmq.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xwm.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uob.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ikk.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hvi.jianghu66.top

[H10] 资源自动释放
来源：http://poh.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mdk.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jmb.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mqz.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gzw.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hkx.cdnleiting.top

Go:   defer f.Close()
来源：http://zhk.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fdp.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lbg.havefunace.top

================================================================================
来源：http://bmc.mhx1999.top

I. 正则表达式
来源：http://ipn.nanxuanxn.top

================================================================================
来源：http://szm.shzxlz.cn

[I01] 判断是否匹配
来源：http://gus.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://prw.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://akw.sxryk.cn

JS:   /\d+/.test(s)
来源：http://qmf.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://fls.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ran.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yah.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://qbd.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rle.zhixingplan.top

[I02] 提取所有匹配
来源：http://tzq.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://uxp.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xca.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cki.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://gfq.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgk.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qor.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://eyv.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eat.gzhubu.top

[I03] 提取捕获分组
来源：http://qbj.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ovh.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwl.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvl.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mtb.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sgx.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gur.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aqa.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://leb.zycfv.cn

[I04] 正则替换
来源：http://aji.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xdm.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://naj.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://txt.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zgu.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pur.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jck.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://pkw.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dho.zhengqikj.top

[I05] 按正则拆分
来源：http://dwf.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wpm.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oyw.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://qqt.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://tjb.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://bxz.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dws.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://erx.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://str.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ofm.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lxc.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dei.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ymu.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xys.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://axs.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iii.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jce.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aca.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://oxt.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://flm.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iac.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zgv.feifeiyinyue.top

TS:   /error/gim
来源：http://eow.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ayj.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oel.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://dcg.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lfj.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://vca.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blp.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hoo.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdf.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpk.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mml.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ede.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://osx.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mav.xylfe.cn

================================================================================
来源：http://soi.zhiwuduotai.top

J. 日期与时间
来源：http://okn.ybcxt.top

================================================================================
来源：http://cqo.fehbvm.com

[J01] 获取当前时间
来源：http://yba.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ars.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mha.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://izh.fzhhl.top

TS:   new Date();  Date.now()
来源：http://nfr.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://tfq.dashuyun.cn

Go:   time.Now()
来源：http://kbr.tanke756.top

Ruby: Time.now
来源：http://lob.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bjo.jinqigufen.top

[J02] 格式化输出
来源：http://yoz.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rak.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gpa.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lza.smart0.xyz

TS:   d.toISOString()
来源：http://abm.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ndz.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://azn.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://etf.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ynn.chenzaomai.com

[J03] 字符串解析为日期
来源：http://dkz.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kgm.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fjk.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://dgy.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://yjv.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zqm.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rvw.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://opj.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ynk.yueranfly.top

[J04] 时间戳与日期互转
来源：http://cql.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://adr.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hiz.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lsc.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pur.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wod.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zhz.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gpd.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uay.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://dpl.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://rgb.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://sdk.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgv.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ztg.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://pax.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sjl.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://svw.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://mbu.gaohongyu789.top

[J06] 计算两时间之差
来源：http://yse.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://elp.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://mzn.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fbs.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxm.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qfp.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://nss.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://lfn.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://mmo.svipenyu.cn

[J07] 比较两个日期
来源：http://xuz.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://roh.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yqf.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zxl.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://jqq.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kyu.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://max.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://jsc.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://kqo.tarul.cn

[J08] 提取年月日与星期
来源：http://kro.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkl.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jnm.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fvp.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yzt.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqs.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bwb.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wsi.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://roq.gaohongyu789.top

[J09] 时区处理
来源：http://sfk.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://niz.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnj.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tsc.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdb.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oes.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://odn.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fzl.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hiw.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://usj.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vpd.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xug.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jej.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dye.fehbvm.com


<!-- 参考信息 -->