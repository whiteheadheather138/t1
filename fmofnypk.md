代发 wailian999

JS:   get name() { return this._name; }
来源：http://ggz.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://hiy.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://utv.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jnc.sufxvd.cn

Ruby: attr_accessor :name
来源：http://gqz.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://gig.havefunace.top

[G12] 对象转字符串
来源：http://pxy.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://cwe.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cib.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://wyk.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://zte.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://xrj.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://can.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://ots.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://ohl.gogol.net.cn

[G13] 判断对象类型
来源：http://vun.hammf.cn

Py:   isinstance(u, User)
来源：http://nam.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://etn.fanxiaobao.xyz

JS:   u instanceof User
来源：http://wto.52xcode.cn

TS:   u instanceof User
来源：http://dju.fzhhl.top

Java: u instanceof User
来源：http://gsf.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lib.pycfn.com

Ruby: u.is_a?(User)
来源：http://zaf.zhengqikj.top

C#:   u is User
来源：http://stk.guowangkeji.top

[G14] 数据类 / record
来源：http://edu.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://amh.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://rnn.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://rxk.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://njf.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://huf.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://yvt.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://phb.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://yiy.ydzc1.top

[G15] 枚举
来源：http://kqn.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://upy.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgb.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kem.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://spi.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://zml.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vje.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://qua.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://njl.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://tqk.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vmr.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://ken.meibo888.top

JS:   Object.entries(obj)
来源：http://jqw.zhengqikj.top

TS:   Object.entries(obj)
来源：http://ovx.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fgi.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fmb.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://smg.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://cyy.haohaochexian.top

================================================================================
来源：http://xlp.ehwqpu.com

H. 异常与错误处理
来源：http://zih.0kj1m.cn

================================================================================
来源：http://rsh.gaohongyu789.top

[H01] try / catch 基础
来源：http://hei.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://shl.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://obc.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qez.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lqy.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yal.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zew.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ids.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zhz.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://ldt.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://igb.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rlg.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zst.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ktd.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ihl.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qgv.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://evl.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vpc.shzxlz.cn

[H03] 主动抛出异常
来源：http://bao.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://zrs.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ebl.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://btl.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://ylv.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xhl.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wvh.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yij.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://ytb.gzhubu.top

[H04] 自定义异常类型
来源：http://uwo.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://pwi.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://biy.yj20258888.top

JS:   class MyError extends Error {}
来源：http://usb.andypj.xyz

TS:   class MyError extends Error {}
来源：http://zyn.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://ktp.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qrl.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://ijw.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://yve.epnwcf.com

[H05] 捕获特定类型
来源：http://asn.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://fzf.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbt.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://vvx.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://gyk.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://siv.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dgq.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://hoz.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mvy.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://kee.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://mqh.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iwd.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://qjh.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cxx.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kep.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://umz.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://ood.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://xfj.ywan-chungtsiang.top

[H07] 断言
来源：http://qdi.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://tgx.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://slr.yvedp.cn

JS:   console.assert(x > 0);
来源：http://bwh.cheryme.top

TS:   console.assert(x > 0);
来源：http://eth.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://eag.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rej.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lxy.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://gko.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://yqa.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://lkb.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vrn.cucudq.cn

JS:   e.message;  e.stack
来源：http://inr.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hdc.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jkw.chenjidiqi.icu

Go:   err.Error()
来源：http://lva.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://zfw.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://mdg.sxryk.cn

[H09] 带错误码的异常
来源：http://qcn.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xag.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dzi.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jul.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qph.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lnz.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gmh.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://pvy.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pas.gotoacloud.top

[H10] 资源自动释放
来源：http://cja.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xmp.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bcb.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lar.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vmn.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jar.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://ecs.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sas.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ctl.guannengcc.top

================================================================================
来源：http://jcg.xingfuxueyuan.xyz

I. 正则表达式
来源：http://vtr.sweek.top

================================================================================
来源：http://muh.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://jwc.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ily.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://ovg.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://loz.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://uny.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sfz.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zuy.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://dte.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zbt.cheryme.top

[I02] 提取所有匹配
来源：http://fjn.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://ide.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://caa.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jbd.ivvv.top

TS:   s.match(/\d+/g)
来源：http://max.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wfz.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lya.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://ruk.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wwv.xinyue.icu

[I03] 提取捕获分组
来源：http://nvv.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ocf.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eiz.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfv.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pkj.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ies.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lpg.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ade.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xin.hesvh.cn

[I04] 正则替换
来源：http://jay.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kns.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jvj.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nng.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hjv.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://kyg.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ztd.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mgp.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jzs.yvedp.cn

[I05] 按正则拆分
来源：http://sdm.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://edb.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xgv.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://nfv.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://gvd.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://ixq.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tno.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://der.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gyc.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mit.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jvd.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mgd.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xmw.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxc.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pzx.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tge.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ljo.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blz.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://qlb.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ybh.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lls.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dwu.daxiang520.top

TS:   /error/gim
来源：http://acy.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://msw.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hcq.birdmap.top

Ruby: s.scan(/error/i)
来源：http://ybl.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vck.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://ala.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tyv.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qmw.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxy.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xub.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xav.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://opp.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://typ.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wgc.wangdashe.top

================================================================================
来源：http://bjv.smart0.xyz

J. 日期与时间
来源：http://lyp.shangyingyoupin.top

================================================================================
来源：http://smz.daxiang520.top

[J01] 获取当前时间
来源：http://upr.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jlu.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gxa.sweek.top

JS:   new Date();  Date.now()
来源：http://ssv.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://uvl.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jml.zhoulong.xyz

Go:   time.Now()
来源：http://aqe.fktsv.cn

Ruby: Time.now
来源：http://myh.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ygd.yvedp.cn

[J02] 格式化输出
来源：http://mad.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nvx.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uha.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xqa.feifeiyinyue.top

TS:   d.toISOString()
来源：http://nwn.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rub.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ifg.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ccs.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sxo.svipenyu.cn

[J03] 字符串解析为日期
来源：http://kyb.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cea.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sqi.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://jlp.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://mvf.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ejf.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cld.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://xsd.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ebv.tanke756.top

[J04] 时间戳与日期互转
来源：http://ouv.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qyc.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gey.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mop.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://csv.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rjl.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://den.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wgs.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fvz.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://mse.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://ltz.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vty.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qiy.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzh.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://wtq.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fxa.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://rke.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://soe.zhixingplan.top

[J06] 计算两时间之差
来源：http://mjb.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://bae.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://anw.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://exo.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rkc.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://lls.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://hdo.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://eru.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://aoq.hysaishi.cn

[J07] 比较两个日期
来源：http://wpj.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://aai.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qif.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bex.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://wuo.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://day.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drn.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://zga.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://tqh.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://ssu.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wpa.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://thz.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aud.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zga.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ply.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pcd.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tcq.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://thh.ydjk.org.cn

[J09] 时区处理
来源：http://pik.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qkz.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://etu.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ajh.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://teb.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://brt.zhijiandao.cn


<!-- 参考信息 -->