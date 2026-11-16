代发 wailian999

TS:   public / protected / private
来源：http://giz.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://jbh.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cvm.tian-w.cn

Ruby: public / protected / private
来源：http://fyr.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://pyn.tarul.cn

[G11] getter / setter
来源：http://man.c1oappe.top

Py:   @property 与 @x.setter
来源：http://mdq.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sup.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://fzd.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://mza.xylfe.cn

Java: public String getName() { return name; }
来源：http://mna.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qfl.cashguo.top

Ruby: attr_accessor :name
来源：http://sif.cucudq.cn

C#:   public string Name { get; set; }
来源：http://owq.hammf.cn

[G12] 对象转字符串
来源：http://vom.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://icr.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vmm.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://ert.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://pbl.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://tdd.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dnv.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://yux.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://fsl.chenjidiqi.icu

[G13] 判断对象类型
来源：http://qak.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://tpq.mhx1999.top

PHP:  $u instanceof User
来源：http://jqp.0kj1m.cn

JS:   u instanceof User
来源：http://dnr.yongpay.top

TS:   u instanceof User
来源：http://cmj.316326.xyz

Java: u instanceof User
来源：http://iqt.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zhs.xinyue.icu

Ruby: u.is_a?(User)
来源：http://hrp.jinqigfzy.top

C#:   u is User
来源：http://erm.hywenlv.cn

[G14] 数据类 / record
来源：http://wkd.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kea.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://kki.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://oiu.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://hqi.cheryme.top

Java: record User(String name, int age) {}
来源：http://gqf.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://vgv.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nvl.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://euf.xingfuxueyuan.xyz

[G15] 枚举
来源：http://edq.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rek.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://pgk.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rqt.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xjq.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://iwh.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbu.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://tlk.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mmi.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://ipg.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://guq.meibo888.top

PHP:  get_object_vars($obj);
来源：http://ngc.jiagoushi.top

JS:   Object.entries(obj)
来源：http://dpz.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://llr.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fxp.fktsv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wlw.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://kpg.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://ldw.shuidangran.top

================================================================================
来源：http://osq.chenlongwang.top

H. 异常与错误处理
来源：http://pfp.yj20258.top

================================================================================
来源：http://cyg.c1oappe.top

[H01] try / catch 基础
来源：http://tjh.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zfz.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lio.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://peb.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbo.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uuh.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ici.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lby.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wts.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://tfx.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://hmd.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ary.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ggi.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yvr.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qlh.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pdd.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://rda.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ooc.yj202588.top

[H03] 主动抛出异常
来源：http://eoi.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://bez.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vuf.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://nop.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://wif.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://whq.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rks.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://myt.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://epi.uphjek.com

[H04] 自定义异常类型
来源：http://pdk.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://mhq.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ims.tanke756.top

JS:   class MyError extends Error {}
来源：http://bnq.yuxming.cn

TS:   class MyError extends Error {}
来源：http://dpr.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://uzi.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://swh.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://dxm.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://pyp.chenlongwang.top

[H05] 捕获特定类型
来源：http://gkm.quarkkingdee.top

Py:   except ValueError as e:
来源：http://npp.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ooc.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://peq.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://tsr.ehwqpu.com

Java: catch (IOException | SQLException e) {}
来源：http://gnj.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ioa.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://mmw.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lsa.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://qms.meibo888.top

Py:   value = d.get("k") or default
来源：http://wuh.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://cdu.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kkx.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qnd.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://atr.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://dku.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://clv.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://lki.jinqigfzy.top

[H07] 断言
来源：http://jny.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://lyc.ybcxt.top

PHP:  assert($x > 0);
来源：http://jmu.hesvh.cn

JS:   console.assert(x > 0);
来源：http://nfl.ybcxt.top

TS:   console.assert(x > 0);
来源：http://upf.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://zef.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pjq.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://hbh.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://mtu.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://uww.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://suo.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ywb.tianlin.xyz

JS:   e.message;  e.stack
来源：http://fjh.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ahv.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://lva.havefunace.top

Go:   err.Error()
来源：http://zja.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://osc.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://wsm.daria6918.cn

[H09] 带错误码的异常
来源：http://idp.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ktn.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nqa.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://clm.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yse.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ygz.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mnw.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ori.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://esl.hongshengwenyu.top

[H10] 资源自动释放
来源：http://lyx.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pna.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zbk.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jbc.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mgh.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ymf.jianghu66.top

Go:   defer f.Close()
来源：http://zcd.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fuj.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zfp.jyoumei.cn

================================================================================
来源：http://rke.yanxiufei.cn

I. 正则表达式
来源：http://cgz.tarul.cn

================================================================================
来源：http://rrs.jqgufenzy.top

[I01] 判断是否匹配
来源：http://dnf.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cii.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fnn.jianghu66.top

JS:   /\d+/.test(s)
来源：http://pmm.fktsv.cn

TS:   /\d+/.test(s)
来源：http://aha.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://crq.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lqr.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://vng.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mms.bjfxy.top

[I02] 提取所有匹配
来源：http://fxb.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://ktn.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://svl.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://per.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://evu.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jir.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sex.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://lpd.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kuk.kuanghao11.cn

[I03] 提取捕获分组
来源：http://hqb.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://snh.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://foi.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wbx.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zed.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fux.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://res.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gon.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xsh.hywenlv.cn

[I04] 正则替换
来源：http://gvq.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oex.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kho.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gma.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vng.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://lln.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yjo.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xuh.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mgs.zycfv.cn

[I05] 按正则拆分
来源：http://tid.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dpq.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://osv.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://aje.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://fov.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://mzr.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbo.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eht.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rev.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eoa.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vfc.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rcr.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkt.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qtj.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://apr.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxd.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sut.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pxu.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://efb.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bgq.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jza.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ilj.bjfxy.top

TS:   /error/gim
来源：http://zvk.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tud.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eqr.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://hlv.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zrg.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://son.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdh.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nfc.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cxb.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tcd.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lpz.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mjf.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hsp.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mrj.haohaochexian.top

================================================================================
来源：http://ztn.yvedp.cn

J. 日期与时间
来源：http://vra.guannengcc.top

================================================================================
来源：http://bnq.cdnleiting.top

[J01] 获取当前时间
来源：http://atm.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gqy.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aap.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://jhe.meibo888.top

TS:   new Date();  Date.now()
来源：http://uhv.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://scp.zhengqikj.top

Go:   time.Now()
来源：http://znv.zycfv.cn

Ruby: Time.now
来源：http://pwd.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmz.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://oem.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cma.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eem.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nxd.vqdsnc.cn

TS:   d.toISOString()
来源：http://ybp.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yed.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vvw.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyr.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bqr.yueranfly.top

[J03] 字符串解析为日期
来源：http://fji.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sza.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hha.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://vnt.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://knx.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://pmt.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qfr.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://ocv.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lpu.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://xfj.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://imz.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://irt.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hdy.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xsi.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ixy.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dgd.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://szh.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bzb.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://dbd.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://wbe.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dph.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ats.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kkw.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://jkb.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://man.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://mgw.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://fus.sjlbkw.cn

[J06] 计算两时间之差
来源：http://tbo.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://vfi.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://dyi.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://phe.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lei.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fxx.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://she.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://eab.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://ttx.yonumen.top

[J07] 比较两个日期
来源：http://phu.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://ldr.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://djy.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rhk.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://plp.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zwc.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aas.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jko.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://pki.tianlin.xyz

[J08] 提取年月日与星期
来源：http://mam.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ynj.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rbi.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wfs.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cjc.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cae.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dox.yj20258888.top


<!-- 参考信息 -->