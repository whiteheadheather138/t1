代发 wailian999

TS:   public / protected / private
来源：http://vzq.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://oul.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zqd.ehwqpu.com

Ruby: public / protected / private
来源：http://iij.shzxlz.cn

C#:   public / protected / private / internal
来源：http://wjh.hywenlv.cn

[G11] getter / setter
来源：http://dwi.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://fwl.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xms.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://ptn.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://lxj.tianlin.xyz

Java: public String getName() { return name; }
来源：http://fxv.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ehx.yfazqb.com

Ruby: attr_accessor :name
来源：http://eoa.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://qkx.zdbjq.cn

[G12] 对象转字符串
来源：http://iho.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://dgi.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jvy.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://vyu.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://dnb.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://ptq.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://kvb.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://ulw.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://syp.sxryk.cn

[G13] 判断对象类型
来源：http://twh.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://dwg.cucudq.cn

PHP:  $u instanceof User
来源：http://syw.ydjk.org.cn

JS:   u instanceof User
来源：http://kjt.zhengqikj.top

TS:   u instanceof User
来源：http://zwo.pycfn.com

Java: u instanceof User
来源：http://tpx.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nfg.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://swa.nwbrower.top

C#:   u is User
来源：http://lsn.cqqwz.cn

[G14] 数据类 / record
来源：http://uio.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://crj.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://efg.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://rtt.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://ypo.fehbvm.com

Java: record User(String name, int age) {}
来源：http://lbl.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://ykx.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xkv.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://brd.haohaochexian.top

[G15] 枚举
来源：http://axh.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lxj.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sqh.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ssz.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lyw.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://nls.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://car.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://awj.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lrg.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://voa.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eom.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://thx.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://qxp.zycfv.cn

TS:   Object.entries(obj)
来源：http://gme.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dwq.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://edz.cheryme.top

Ruby: obj.instance_variables
来源：http://rah.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://kcd.gzhubu.top

================================================================================
来源：http://wkj.jinqigufen.top

H. 异常与错误处理
来源：http://fjo.chenzaomai.com

================================================================================
来源：http://uyo.fktsv.cn

[H01] try / catch 基础
来源：http://bez.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vbu.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wbz.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vzd.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ogj.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://itr.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ruc.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pmj.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yrd.nwbrower.top

[H02] finally / ensure 收尾
来源：http://qft.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://loz.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rqx.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fjx.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sqn.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://hja.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://glv.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uzf.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mcg.shuidangran.top

[H03] 主动抛出异常
来源：http://jly.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://mfg.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gay.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://tmo.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://ksw.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ycm.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epl.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mcc.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://kpx.hfpthk.cn

[H04] 自定义异常类型
来源：http://jmw.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://vig.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qpf.fehbvm.com

JS:   class MyError extends Error {}
来源：http://jzx.hnqzz.top

TS:   class MyError extends Error {}
来源：http://fxh.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://tfn.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lkt.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://scc.bbcook.cn

C#:   class MyException : Exception {}
来源：http://fag.gotoacloud.top

[H05] 捕获特定类型
来源：http://dom.quarkkingdee.top

Py:   except ValueError as e:
来源：http://elr.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://enh.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://wqa.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://spp.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://kaq.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nsf.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://rvs.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://paa.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://ysk.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://vhi.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://afd.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://lrk.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jpp.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uhz.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nvv.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://uaf.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://pwk.haohaochexian.top

[H07] 断言
来源：http://vcx.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://uvp.jiagoushi.top

PHP:  assert($x > 0);
来源：http://yil.hcnkem.com

JS:   console.assert(x > 0);
来源：http://njj.meibo888.top

TS:   console.assert(x > 0);
来源：http://jex.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://mzo.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rot.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://acw.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://ucn.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://rqi.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://kdb.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ihx.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://nml.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkf.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vdx.ywan-chungtsiang.top

Go:   err.Error()
来源：http://omm.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://nlc.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://hyf.jqgufenzy.top

[H09] 带错误码的异常
来源：http://xta.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://utj.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fac.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rdi.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://agq.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qku.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zng.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://zln.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xsv.hcnkem.com

[H10] 资源自动释放
来源：http://zrl.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tnv.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pil.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ure.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jpp.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sax.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://jae.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzr.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://clr.redwolf501.top

================================================================================
来源：http://ccr.dianchejie.cn

I. 正则表达式
来源：http://xqa.zhengqikj.top

================================================================================
来源：http://oyu.yueranfly.top

[I01] 判断是否匹配
来源：http://uen.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ndh.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://amo.vehdjk.com

JS:   /\d+/.test(s)
来源：http://lib.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://asq.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gut.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bll.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://cyl.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hib.jqgufenzy.top

[I02] 提取所有匹配
来源：http://qpg.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://ecn.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uoq.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mom.cheryme.top

TS:   s.match(/\d+/g)
来源：http://xat.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://efp.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pkp.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://hhs.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ebo.cashguo.top

[I03] 提取捕获分组
来源：http://agr.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rxx.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yyw.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fml.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zet.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dun.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rqu.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rbw.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ebj.ivvv.top

[I04] 正则替换
来源：http://dnv.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://shu.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://due.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ral.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://dkx.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://sce.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://prc.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://alt.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tnh.yfazqb.com

[I05] 按正则拆分
来源：http://rem.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fzo.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fph.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://lhy.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://qsg.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://cyh.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cxg.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://pqb.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdf.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ouc.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wkw.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ufl.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fkb.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppe.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wsg.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ndn.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xxx.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://olg.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://rab.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xjr.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://chm.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kbi.jianghu66.top

TS:   /error/gim
来源：http://tfh.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sqn.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mxc.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://bwo.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wyz.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://puy.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://azm.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gdp.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hew.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmr.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bny.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mva.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://evi.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bec.chenzaomai.com

================================================================================
来源：http://wwp.yj20258.top

J. 日期与时间
来源：http://wag.ywan-chungtsiang.top

================================================================================
来源：http://hmz.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://vum.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tgx.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yrr.yueranfly.top

JS:   new Date();  Date.now()
来源：http://ird.fktsv.cn

TS:   new Date();  Date.now()
来源：http://hts.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://cpv.hywenlv.cn

Go:   time.Now()
来源：http://hli.cheryme.top

Ruby: Time.now
来源：http://bie.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fko.haohaochexian.top

[J02] 格式化输出
来源：http://jnl.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uix.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bqa.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zhz.meibo888.top

TS:   d.toISOString()
来源：http://cai.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ktg.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iex.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fkd.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yni.ivvv.top

[J03] 字符串解析为日期
来源：http://uhh.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fny.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jyc.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://umm.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://svl.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://ykm.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://szv.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://qyz.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vlb.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://nfg.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kib.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dbv.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xvq.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dyx.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fsp.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mmv.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ywp.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bvt.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://daw.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://wxu.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://flp.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwe.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vrq.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://zjh.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qik.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://pab.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://xxl.aizwys.cn

[J06] 计算两时间之差
来源：http://pvl.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://tno.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://xft.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iou.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ovq.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://aat.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://pch.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://kpe.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://zxm.zhongyouzk.top

[J07] 比较两个日期
来源：http://sbi.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://umc.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ytb.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://xqm.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ejo.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://znd.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gic.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yxx.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://dje.meibo888.top

[J08] 提取年月日与星期
来源：http://eio.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mvy.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tsw.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cdl.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tiv.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sgo.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rrc.xingfuxueyuan.xyz


<!-- 参考信息 -->