代发 wailian999

C#:   public / protected / private / internal
来源：http://ltt.meibo888.top

[G11] getter / setter
来源：http://ggl.yonumen.top

Py:   @property 与 @x.setter
来源：http://rmp.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wmu.yongpay.top

JS:   get name() { return this._name; }
来源：http://ohf.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://kiu.daria6918.cn

Java: public String getName() { return name; }
来源：http://frl.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wdv.daria6918.cn

Ruby: attr_accessor :name
来源：http://jpw.cucudq.cn

C#:   public string Name { get; set; }
来源：http://olx.guannengcc.top

[G12] 对象转字符串
来源：http://win.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://gvd.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://dzn.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://dll.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://xgm.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://biq.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kvq.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://yrs.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://stm.bjfxy.top

[G13] 判断对象类型
来源：http://grk.tanke756.top

Py:   isinstance(u, User)
来源：http://wmd.jinqigfzy.top

PHP:  $u instanceof User
来源：http://wfr.kuanghao11.cn

JS:   u instanceof User
来源：http://shb.zhiwuduotai.top

TS:   u instanceof User
来源：http://hqj.316326.xyz

Java: u instanceof User
来源：http://mza.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mht.tanke756.top

Ruby: u.is_a?(User)
来源：http://iuw.ctjpmb.com

C#:   u is User
来源：http://zrv.jlsjyb.cn

[G14] 数据类 / record
来源：http://cex.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mdj.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://oxn.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://rrt.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://lsg.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://dxv.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://xjp.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://prq.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://jtq.yanxiufei.cn

[G15] 枚举
来源：http://hid.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nxa.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bzu.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mry.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gbe.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://nfb.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzo.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://hgd.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ihm.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://ijy.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kql.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://gro.52xcode.cn

JS:   Object.entries(obj)
来源：http://nka.meibo888.top

TS:   Object.entries(obj)
来源：http://wgl.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iut.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ozf.meibo888.top

Ruby: obj.instance_variables
来源：http://cia.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://cir.havefunace.top

================================================================================
来源：http://pqf.pycfn.com

H. 异常与错误处理
来源：http://nmf.daria6918.cn

================================================================================
来源：http://pmi.redwolf501.top

[H01] try / catch 基础
来源：http://qop.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqn.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://smv.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rxp.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dpz.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mne.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dji.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://acf.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://spn.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://ndw.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://erc.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kyb.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hmt.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qck.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://gxu.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kul.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pnn.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvu.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://qpi.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://hoq.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://asl.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://hgp.yongpay.top

TS:   throw new Error("错误信息");
来源：http://nse.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dyc.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bmz.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://qov.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://rim.quarkkingdee.top

[H04] 自定义异常类型
来源：http://gli.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://xbv.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://dkx.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://wig.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://vrz.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://byo.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://atr.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://jfi.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://dlw.tian-w.cn

[H05] 捕获特定类型
来源：http://lnh.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://vbh.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ggx.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://bye.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://ufz.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://udp.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cwt.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://dlt.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdd.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://vvv.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://dsi.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tfv.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://qdz.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fdm.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cav.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ffy.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://zec.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://upc.shangyingyoupin.top

[H07] 断言
来源：http://axs.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://umd.gogol.net.cn

PHP:  assert($x > 0);
来源：http://kpr.yueranfly.top

JS:   console.assert(x > 0);
来源：http://vut.vehdjk.com

TS:   console.assert(x > 0);
来源：http://ybz.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://pbn.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vnz.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://thu.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://rbc.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://xsx.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://ujs.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://byb.zhixingplan.top

JS:   e.message;  e.stack
来源：http://sly.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eqn.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mew.zhaomingkeji.xyz

Go:   err.Error()
来源：http://ofr.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://rru.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://rgv.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://otz.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nsg.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rjf.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://huz.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kol.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxd.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nse.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ygq.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cim.meibo888.top

[H10] 资源自动释放
来源：http://lzm.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nck.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bzu.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ibm.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qas.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xnk.nwbrower.top

Go:   defer f.Close()
来源：http://ztq.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gct.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zem.jianghu66.top

================================================================================
来源：http://aqw.zhijiandao.cn

I. 正则表达式
来源：http://ems.sweek.top

================================================================================
来源：http://fig.zhengqikj.top

[I01] 判断是否匹配
来源：http://nbx.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://crx.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fil.yvedp.cn

JS:   /\d+/.test(s)
来源：http://eni.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://dym.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ewt.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ycg.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://pod.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nwh.yvedp.cn

[I02] 提取所有匹配
来源：http://uqu.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://elr.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://stn.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jen.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://pcn.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://flv.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qbi.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://mqc.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mif.zhoulong.xyz

[I03] 提取捕获分组
来源：http://anl.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gts.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xjy.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pzb.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://myx.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://att.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://csv.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wfk.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pyq.9152youxi.cn

[I04] 正则替换
来源：http://mkx.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://cod.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gjn.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://kof.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://tuv.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fcb.chenzaomai.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fxy.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dob.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://acn.fzhhl.top

[I05] 按正则拆分
来源：http://hez.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yfd.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lzf.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://cxy.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://vpm.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://eyl.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ten.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://pxp.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jey.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rha.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://par.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hdg.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bwt.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bwx.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tug.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kcb.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://isw.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://icc.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://xxi.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jsl.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://doj.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mer.jianghu66.top

TS:   /error/gim
来源：http://xet.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ysu.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qst.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://aoq.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hdt.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://kpn.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qfh.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sjc.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://plp.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://waq.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://puh.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hdv.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://owa.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jic.yfazqb.com

================================================================================
来源：http://kuj.aizwys.cn

J. 日期与时间
来源：http://lte.daxiang520.top

================================================================================
来源：http://eit.hysaishi.cn

[J01] 获取当前时间
来源：http://ing.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hgz.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gft.52xcode.cn

JS:   new Date();  Date.now()
来源：http://wnb.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://ndm.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nvd.aizwys.cn

Go:   time.Now()
来源：http://lkf.tianlin.xyz

Ruby: Time.now
来源：http://xgn.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yiu.fanxiaobao.xyz

[J02] 格式化输出
来源：http://xvk.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uiv.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ilo.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cor.zhongyouzk.top

TS:   d.toISOString()
来源：http://sma.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hrk.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bcb.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wef.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://txj.hcnkem.com

[J03] 字符串解析为日期
来源：http://kwu.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kzl.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fan.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://wpd.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://aci.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://mai.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dok.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://bfd.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nas.tarul.cn

[J04] 时间戳与日期互转
来源：http://jfh.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ntj.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ogx.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zvv.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://aod.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vqk.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fey.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qrc.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jyt.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://zdd.havefunace.top

Py:   now + timedelta(days=7)
来源：http://wqk.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://tiz.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzc.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nup.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://pqo.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vcg.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://orb.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://pkf.ydjk.org.cn

[J06] 计算两时间之差
来源：http://ihh.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://fvu.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://ajc.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eum.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xda.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://stl.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://acx.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://pll.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://jhx.shzxlz.cn

[J07] 比较两个日期
来源：http://bab.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://eyq.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mus.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ogt.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vgb.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ciy.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oeg.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://ixn.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://vqk.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://liu.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eiu.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xeb.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rol.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uyq.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nfs.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhb.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vly.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdd.yonumen.top

[J09] 时区处理
来源：http://kvo.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ldt.jiagoushi.top


<!-- 参考信息 -->