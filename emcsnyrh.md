代发 wailian999

[G10] 访问控制
来源：http://juu.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://cja.hnxiangtu.top

PHP:  public / protected / private
来源：http://gpf.tarul.cn

JS:   #private 字段；其余公开
来源：http://daq.wangdashe.top

TS:   public / protected / private
来源：http://hcn.hammf.cn

Java: public / protected / private / 默认包级
来源：http://xbk.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://woq.epnwcf.com

Ruby: public / protected / private
来源：http://hzd.haohaochexian.top

C#:   public / protected / private / internal
来源：http://iuj.dashuyun.cn

[G11] getter / setter
来源：http://psm.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://ogv.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nyh.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://fjc.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://zqg.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://zwd.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnb.snrcjt.cn

Ruby: attr_accessor :name
来源：http://vgy.shuidangran.top

C#:   public string Name { get; set; }
来源：http://sdd.iojbl.cn

[G12] 对象转字符串
来源：http://jpi.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://xdp.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wxv.cucudq.cn

JS:   toString() { return this.name; }
来源：http://xdz.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://lgt.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://dbi.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://vrd.birdmap.top

Ruby: def to_s; @name; end
来源：http://rds.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ost.yuanzhike.top

[G13] 判断对象类型
来源：http://iuj.jiagoushi.top

Py:   isinstance(u, User)
来源：http://hhg.vehdjk.com

PHP:  $u instanceof User
来源：http://hic.pycfn.com

JS:   u instanceof User
来源：http://pbb.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://gbf.fanxiaobao.xyz

Java: u instanceof User
来源：http://yyj.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fbe.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://xvd.yanxiufei.cn

C#:   u is User
来源：http://scj.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://yyt.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mbj.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://fbq.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qwr.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://fdu.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://nxh.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://kvq.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jzu.uphjek.com

C#:   record User(string Name, int Age);
来源：http://pha.wangdashe.top

[G15] 枚举
来源：http://wmd.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kub.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bzr.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zqp.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://boh.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://ure.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgp.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://ipc.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fwg.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://sdj.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kbp.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://wgk.cqqwz.cn

JS:   Object.entries(obj)
来源：http://dbf.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://jjs.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qvn.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zyw.meibo888.top

Ruby: obj.instance_variables
来源：http://axp.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://oyp.snrcjt.cn

================================================================================
来源：http://vua.smart0.xyz

H. 异常与错误处理
来源：http://wyp.gaohongyu789.top

================================================================================
来源：http://cbw.guannengcc.top

[H01] try / catch 基础
来源：http://ubz.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bor.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wtd.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kcu.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fsr.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://upw.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwr.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pnf.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lcv.sxryk.cn

[H02] finally / ensure 收尾
来源：http://jje.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://srp.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ilj.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mie.chenjidiqi.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://dxd.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://uff.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xcm.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mur.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjy.jqgfzy.top

[H03] 主动抛出异常
来源：http://zyd.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://pxb.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wlq.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://vdj.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://gxf.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zck.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gum.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://bpw.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vsg.hfpthk.cn

[H04] 自定义异常类型
来源：http://rvo.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://xbx.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://jpl.bbcook.cn

JS:   class MyError extends Error {}
来源：http://dyn.ybcxt.top

TS:   class MyError extends Error {}
来源：http://tkv.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://rae.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://itj.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://sph.smart0.xyz

C#:   class MyException : Exception {}
来源：http://itn.0kj1m.cn

[H05] 捕获特定类型
来源：http://yqz.pycfn.com

Py:   except ValueError as e:
来源：http://fpf.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sfg.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://kwk.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://nul.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://mbm.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://izq.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://kbe.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vtw.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://zfa.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://dca.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://thj.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://wqp.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://awm.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nud.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://dpg.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://ujk.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://uki.guannengcc.top

[H07] 断言
来源：http://boz.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://ddv.cashguo.top

PHP:  assert($x > 0);
来源：http://itq.yonumen.top

JS:   console.assert(x > 0);
来源：http://qne.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://fug.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://yky.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tzn.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://sen.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://fnu.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://tda.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://uhm.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iac.aizwys.cn

JS:   e.message;  e.stack
来源：http://utm.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kyi.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://gcp.jyoumei.cn

Go:   err.Error()
来源：http://zcc.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://pje.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://nxq.aizwys.cn

[H09] 带错误码的异常
来源：http://zyx.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://div.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vaz.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwt.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mtd.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hwh.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ahf.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://xwd.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nrg.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://evv.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ljn.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kss.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gbl.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xuw.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ssv.yongpay.top

Go:   defer f.Close()
来源：http://uds.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://msq.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lpq.ydjk.org.cn

================================================================================
来源：http://ckp.zhengqikj.top

I. 正则表达式
来源：http://cjp.sufxvd.cn

================================================================================
来源：http://efa.jinqigufen.top

[I01] 判断是否匹配
来源：http://sbz.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://moc.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://mwe.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://amo.guannengcc.top

TS:   /\d+/.test(s)
来源：http://xgg.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uhv.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gpi.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://yng.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wfd.c1oappe.top

[I02] 提取所有匹配
来源：http://wty.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://fef.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rvo.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sju.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://ylw.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vjg.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://llv.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://ujd.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jkn.52xcode.cn

[I03] 提取捕获分组
来源：http://vqy.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vcs.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nym.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bxa.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tbf.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jld.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mwv.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tvt.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://guz.zhiwuduotai.top

[I04] 正则替换
来源：http://nya.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ilb.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ybk.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xfz.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://imv.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lys.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://efq.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gzm.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uza.cashguo.top

[I05] 按正则拆分
来源：http://xiu.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://woz.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xco.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://klz.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://jjw.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://bbw.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pxn.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://pfv.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://trm.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://djc.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mzy.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ppu.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mjc.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzw.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hfg.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://chz.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vxh.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hjt.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://jkp.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kgh.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mxx.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jxa.cashguo.top

TS:   /error/gim
来源：http://emx.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xcm.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rxr.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://xdq.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gdo.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://lmo.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imo.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zbs.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dts.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wjg.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngp.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hhy.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lfx.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://auy.aibaodan.cn

================================================================================
来源：http://lnf.sysykeji.top

J. 日期与时间
来源：http://rtp.sweek.top

================================================================================
来源：http://uqa.feifeiyinyue.top

[J01] 获取当前时间
来源：http://vqi.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zqx.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://huw.yuxming.cn

JS:   new Date();  Date.now()
来源：http://odi.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://nyu.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zcy.havefunace.top

Go:   time.Now()
来源：http://trl.guowangkeji.top

Ruby: Time.now
来源：http://rpf.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uis.yanxiufei.cn

[J02] 格式化输出
来源：http://bqr.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lpd.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uex.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cif.xuetiantiany.cn

TS:   d.toISOString()
来源：http://rze.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://flp.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fdq.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hfx.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://whc.snrcjt.cn

[J03] 字符串解析为日期
来源：http://hli.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fec.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wln.cheryme.top

JS:   new Date("2024-01-02")
来源：http://hvw.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://wha.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://xim.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mmg.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://zck.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rmb.xylfe.cn

[J04] 时间戳与日期互转
来源：http://tqp.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://say.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ylv.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gms.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qzt.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kat.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aef.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wgh.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wfh.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://dfi.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://sww.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jki.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oeb.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mkr.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://jjc.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mca.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://qkf.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://mmm.iojbl.cn

[J06] 计算两时间之差
来源：http://qle.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://lce.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://eem.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dpf.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ucb.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xlq.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://aos.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://crh.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://hpk.bbcook.cn

[J07] 比较两个日期
来源：http://cgh.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://kjz.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lba.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vdp.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://snl.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tec.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jwh.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://hdc.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://acj.tian-w.cn

[J08] 提取年月日与星期
来源：http://ucs.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ifd.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qkf.yonumen.top


<!-- 参考信息 -->