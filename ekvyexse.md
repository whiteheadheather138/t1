代发 wailian999

TS:   public / protected / private
来源：http://dfi.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://hrk.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oom.daria6918.cn

Ruby: public / protected / private
来源：http://udx.316326.xyz

C#:   public / protected / private / internal
来源：http://mjq.c1oappe.top

[G11] getter / setter
来源：http://grc.yuxming.cn

Py:   @property 与 @x.setter
来源：http://krq.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pmb.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://xjb.sweek.top

TS:   get name(): string { return this._name; }
来源：http://vuu.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://kro.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://blk.aibaodan.cn

Ruby: attr_accessor :name
来源：http://oao.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://bvi.316326.xyz

[G12] 对象转字符串
来源：http://vyo.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://mgg.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rmd.fehbvm.com

JS:   toString() { return this.name; }
来源：http://hcr.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://mgv.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://ajl.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://rzd.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://qmc.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://xuy.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://qrw.hcnkem.com

Py:   isinstance(u, User)
来源：http://rei.hesvh.cn

PHP:  $u instanceof User
来源：http://bzw.cheryme.top

JS:   u instanceof User
来源：http://ufq.ctjpmb.com

TS:   u instanceof User
来源：http://gll.gotoacloud.top

Java: u instanceof User
来源：http://ucw.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdj.yuxming.cn

Ruby: u.is_a?(User)
来源：http://ycc.yonumen.top

C#:   u is User
来源：http://mof.zhengqikj.top

[G14] 数据类 / record
来源：http://tej.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rfg.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://npg.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://rno.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://gwe.yueranfly.top

Java: record User(String name, int age) {}
来源：http://nqa.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://ahm.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyh.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://ser.zhiwuduotai.top

[G15] 枚举
来源：http://obj.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eio.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rco.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ibi.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://obw.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://mof.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://crw.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://axl.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nzm.meibo888.top

[G16] 对象转数组 / 字典
来源：http://txq.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tde.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://alq.snrcjt.cn

JS:   Object.entries(obj)
来源：http://ovj.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://lhg.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ldk.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jev.ppjwa.cn

Ruby: obj.instance_variables
来源：http://ukh.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://tyv.dashuyun.cn

================================================================================
来源：http://hnx.pengpengdd.cyou

H. 异常与错误处理
来源：http://pxs.cdnleiting.top

================================================================================
来源：http://goo.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://edl.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sgt.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nqg.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bed.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pat.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wex.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vhx.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://phw.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://izj.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://tgh.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://lwd.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wxz.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://btw.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kum.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cpt.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://guj.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ket.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vpa.bbcook.cn

[H03] 主动抛出异常
来源：http://pwv.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://skx.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ukc.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://acn.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://gsf.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://paq.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tgl.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rsf.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://fnh.quarkkingdee.top

[H04] 自定义异常类型
来源：http://slf.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://kwi.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://vvu.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://btl.52xcode.cn

TS:   class MyError extends Error {}
来源：http://zjj.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://bef.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qph.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://cam.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://gia.zhengqikj.top

[H05] 捕获特定类型
来源：http://bcj.sweek.top

Py:   except ValueError as e:
来源：http://hzf.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rig.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://bff.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://xfz.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://cpd.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yrw.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://doy.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tuh.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://yht.tarul.cn

Py:   value = d.get("k") or default
来源：http://hho.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qgl.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://wsp.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://idc.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cjz.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xcc.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://iwq.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://xzg.yvedp.cn

[H07] 断言
来源：http://vlp.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://ryh.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://baw.mhx1999.top

JS:   console.assert(x > 0);
来源：http://mly.mhx1999.top

TS:   console.assert(x > 0);
来源：http://xli.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://cdz.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xtb.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://qjn.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://sjr.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://xkn.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://grv.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://owt.xuetiantiany.cn

JS:   e.message;  e.stack
来源：http://eue.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://onj.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dvh.sysykeji.top

Go:   err.Error()
来源：http://pvk.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://szx.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://mix.sxryk.cn

[H09] 带错误码的异常
来源：http://qia.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nuu.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://fvx.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cdt.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vep.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wma.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://knu.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://ktg.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kad.ivvv.top

[H10] 资源自动释放
来源：http://yjt.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dib.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rjl.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hae.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jyu.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lnl.dashuyun.cn

Go:   defer f.Close()
来源：http://fcs.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wyf.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sdn.nanxuanxn.top

================================================================================
来源：http://vzs.hywenlv.cn

I. 正则表达式
来源：http://fad.jqgufenzy.top

================================================================================
来源：http://iqt.cucudq.cn

[I01] 判断是否匹配
来源：http://jow.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gtp.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://nfz.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://ycv.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://rhw.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ipd.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ypw.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://ygf.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dcs.aizwys.cn

[I02] 提取所有匹配
来源：http://vpa.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://qpr.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bnr.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hov.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://jxc.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nso.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dfh.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://jjf.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zjm.cdnleiting.top

[I03] 提取捕获分组
来源：http://stq.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uxw.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hnh.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ulg.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eap.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rbk.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kyh.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lhz.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yic.mhx1999.top

[I04] 正则替换
来源：http://jqi.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wjr.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lqg.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ftw.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://crr.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://ccb.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ekm.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tcg.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uth.wangdashe.top

[I05] 按正则拆分
来源：http://txl.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mei.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dty.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://hww.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://glk.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://jnx.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rrz.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qun.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zit.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xrz.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ynz.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ven.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqd.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://otp.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ujg.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qaf.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gbx.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nbt.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://xxw.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uxl.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://asf.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://igo.bbcook.cn

TS:   /error/gim
来源：http://agw.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pow.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kql.yj20258.top

Ruby: s.scan(/error/i)
来源：http://oov.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://evd.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ygn.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bjp.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tzp.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://adq.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jwf.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cxy.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pud.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://euc.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://llp.316326.xyz

================================================================================
来源：http://bcv.sxryk.cn

J. 日期与时间
来源：http://djl.jqgfzy.top

================================================================================
来源：http://jhh.guannengcc.top

[J01] 获取当前时间
来源：http://uch.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zdz.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vvk.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://dbk.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://aiw.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cuh.yueranfly.top

Go:   time.Now()
来源：http://ntn.c1oappe.top

Ruby: Time.now
来源：http://fdh.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vpg.ydjk.org.cn

[J02] 格式化输出
来源：http://igb.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhs.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lew.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ouc.316326.xyz

TS:   d.toISOString()
来源：http://dut.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ylv.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rrx.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wgn.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hwf.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://plh.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yys.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dxp.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://bek.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://iun.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://uug.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvk.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://bkv.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nny.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://gow.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rtp.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewf.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cfb.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bnj.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dvc.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cga.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://quc.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ooj.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://szk.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://rvo.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jxq.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hyo.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://apy.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://fex.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bik.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://zps.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://gcf.zhixingplan.top

[J06] 计算两时间之差
来源：http://yue.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://qye.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://kbm.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eyk.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ytz.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://vep.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://izh.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://kyp.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://htp.shzxlz.cn

[J07] 比较两个日期
来源：http://kok.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://khj.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pym.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://qeh.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://glo.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rzm.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bih.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://txm.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://txy.meibo888.top

[J08] 提取年月日与星期
来源：http://ptw.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvd.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dvq.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://grc.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mgg.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://omv.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pxv.pengpengdd.cyou


<!-- 参考信息 -->