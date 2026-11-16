代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wdt.jyoumei.cn

[Q75] 日期格式化
来源：http://bsd.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jny.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://stq.yj202588.top

[Q76] 按天统计
来源：http://eff.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fmk.fengsongda.top

[Q77] 时间加减
来源：http://pmt.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mwr.tanke756.top

[Q78] 当前时间
来源：http://xrk.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kay.daria6918.cn

[Q79] 字符串拼接
来源：http://nya.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pwv.jyoumei.cn

[Q80] 字符串截取
来源：http://rga.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fda.nanxinkj.top

[Q81] 字符串替换
来源：http://ien.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uon.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://mni.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cas.ehwqpu.com

[Q83] 大小写转换
来源：http://qzn.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oft.hysaishi.cn

[Q84] 去除首尾空格
来源：http://nmq.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://bpd.hcnkem.com

[Q85] 数值取整
来源：http://yrq.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qxc.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://hkr.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://voy.316326.xyz

[Q87] JSON 字段做条件
来源：http://zjj.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://csp.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://llp.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mjt.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ryj.haohaochexian.top

[Q89] 判断表是否存在
来源：http://esc.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kao.xuanzx.com

[Q90] 生成序号列
来源：http://fbc.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uip.andypj.xyz

================================================================================
来源：http://cfx.hongshengwenyu.top

R. Bash 专题
来源：http://pul.shangyingyoupin.top

================================================================================
来源：http://fsp.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://hgj.yueranfly.top

#!/usr/bin/env bash
来源：http://wyl.ppjwa.cn

set -euo pipefail
来源：http://xox.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://iih.guannengcc.top

name="Tom"; echo "$name"
来源：http://von.c1oappe.top

[R03] 只读变量
来源：http://zfa.redwolf501.top

readonly PI=3.14
来源：http://fjy.jlsjyb.cn

[R04] 位置参数
来源：http://yhj.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wbl.fehbvm.com

[R05] 参数默认值
来源：http://ngx.zhiwuduotai.top

name="${1:-default}"
来源：http://zzk.gzhubu.top

[R06] 判断命令是否存在
来源：http://pge.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qxn.yonumen.top

[R07] if 判断文件
来源：http://yzz.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wgu.dashuyun.cn

[R08] 数值比较
来源：http://frb.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qmn.tian-w.cn

[R09] 字符串比较
来源：http://liq.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nxi.fehbvm.com

[R10] 正则匹配
来源：http://mow.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aep.fehbvm.com

[R11] case 多分支
来源：http://rqc.uphjek.com

case "$1" in
来源：http://opk.zhixingplan.top

start) echo "启动" ;;
来源：http://luj.fzhhl.top

stop)  echo "停止" ;;
来源：http://zlv.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://lif.xziqi.cn

esac
来源：http://nxh.havefunace.top

[R12] for 遍历文件
来源：http://enk.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://nbl.yonumen.top

[R13] for 计数循环
来源：http://lga.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://aux.316326.xyz

[R14] C 风格 for
来源：http://qzg.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ium.yuxming.cn

[R15] while 逐行读文件
来源：http://htl.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xln.yongpay.top

[R16] until 等待条件
来源：http://usm.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jpx.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://xkd.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gas.dashuyun.cn

[R18] 遍历数组
来源：http://lzg.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wqt.cucudq.cn

[R19] 数组长度
来源：http://zkk.svipenyu.cn

echo "${#arr[@]}"
来源：http://tlm.cdnleiting.top

[R20] 关联数组（字典）
来源：http://vcr.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sue.jiagoushi.top

[R21] 字符串长度
来源：http://jzw.jqgfzy.top

echo "${#s}"
来源：http://zvk.meibo888.top

[R22] 截取子串
来源：http://amw.jqgufenzy.top

echo "${s:0:5}"
来源：http://njw.quarkkingdee.top

[R23] 字符串替换
来源：http://qxq.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fcf.nanxinkj.top

[R24] 大小写转换
来源：http://wnh.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://oqz.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://zqw.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxc.dianchejie.cn

[R26] 命令替换
来源：http://mfx.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://umb.zdqjudy.top

[R27] 算术展开
来源：http://mxy.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://sim.ivvv.top

[R28] 浮点运算
来源：http://zhf.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://tby.hcnkem.com

[R29] 定义函数
来源：http://jzl.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://red.nwbrower.top

[R30] 函数返回状态码
来源：http://hii.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://oqy.redwolf501.top

[R31] 局部变量
来源：http://xdr.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://hih.jqgufenzy.top

[R32] 参数个数校验
来源：http://nhy.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mss.uphjek.com

[R33] 捕获错误并提示行号
来源：http://nnr.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nje.svipenyu.cn

[R34] 退出时清理
来源：http://hmo.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://sbe.ydzc1.top

[R35] 后台执行并等待
来源：http://pci.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pcr.bbcook.cn

[R36] 并发执行多个任务
来源：http://njw.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://crh.hywenlv.cn

[R37] 把输出赋给变量
来源：http://mhv.tianlin.xyz

files=$(ls -1)
来源：http://bmp.haohaochexian.top

[R38] 管道串联
来源：http://hph.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://wjc.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://jca.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://hxl.aizwys.cn

[R40] 追加写日志
来源：http://yjl.pengpengdd.cyou

echo "log" >> out.log
来源：http://akg.gzhubu.top

[R41] 丢弃输出
来源：http://rll.pycfn.com

cmd >/dev/null 2>&1
来源：http://lyl.ydjk.org.cn

[R42] 输入重定向
来源：http://jix.hnqzz.top

wc -l < a.txt
来源：http://lfv.zycfv.cn

[R43] 按名字查找文件
来源：http://unq.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://atv.52xcode.cn

[R44] 按修改时间查找
来源：http://yjr.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://gyb.hesvh.cn

[R45] 批量删除
来源：http://wwl.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://yht.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://cnb.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://adn.xylfe.cn

[R47] sed 单行替换
来源：http://kya.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://ary.cdnleiting.top

[R48] awk 取指定列
来源：http://aka.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://ntq.yj202588.top

[R49] awk 带条件
来源：http://jrt.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xkx.pengpengdd.cyou

[R50] awk 求和
来源：http://ggq.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pqb.yanxiufei.cn

[R51] 排序去重取前几
来源：http://evc.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://soo.mhx1999.top

[R52] 统计行数
来源：http://mfe.daxiang520.top

wc -l a.txt
来源：http://jhd.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://veh.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bkm.ehwqpu.com

[R54] 比较两个文件
来源：http://rxq.yueranfly.top

diff a.txt b.txt
来源：http://ogu.ehwqpu.com

[R55] 压缩与解压
来源：http://vqu.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://meh.yuxming.cn

[R56] 远程拷贝
来源：http://hmb.shuidangran.top

scp file user@host:/path/
来源：http://jtp.hnqzz.top

[R57] 远程执行命令
来源：http://gnj.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://ttq.shuidangran.top

[R58] 下载文件
来源：http://vyu.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wla.vqdsnc.cn

[R59] 发 POST JSON
来源：http://lzo.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ilg.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://jgg.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qfm.zhiwuduotai.top

[R61] 磁盘占用
来源：http://pca.ybcxt.top

df -h;  du -sh *
来源：http://znv.tian-w.cn

[R62] 找最占空间的文件
来源：http://vor.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://zht.jianghu66.top

[R63] 内存与进程
来源：http://kdy.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://yvj.zdqjudy.top

[R64] 结束进程
来源：http://xub.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://pgq.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://fgz.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wwf.nanxuanxn.top

[R66] 定时任务
来源：http://ain.iojbl.cn

crontab -e;  crontab -l
来源：http://ryy.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://nam.sxryk.cn

openssl rand -hex 16
来源：http://lsu.c1oappe.top

[R68] 计算文件校验值
来源：http://yot.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://xkg.cashguo.top

[R69] 生成随机密码
来源：http://jeq.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://lgg.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://pnn.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://whv.kuanghao11.cn

[R71] 日期格式化
来源：http://duw.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sgh.zdqjudy.top

[R72] 等待端口就绪
来源：http://eeq.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ovn.316326.xyz

[R73] 分割大日志
来源：http://ruj.bjfxy.top

split -l 1000 big.log part_
来源：http://lko.ctjpmb.com

[R74] 批量重命名
来源：http://wuw.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://suh.nanxuanxn.top

[R75] 导出环境变量
来源：http://uqe.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://dhl.sjlbkw.cn

[R76] 使用临时文件
来源：http://lnj.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zkw.jlsjyb.cn

[R77] 读取用户输入
来源：http://owj.tarul.cn

read -rp "请输入: " ans
来源：http://kro.ydjk.org.cn

[R78] 交互式菜单
来源：http://oek.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ogf.epnwcf.com

[R79] 解析命令行选项
来源：http://ngi.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://riv.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://caf.zhijiandao.cn

time ./run.sh
来源：http://gyj.hnqzz.top

================================================================================
来源：http://tfd.pengpengdd.cyou

S. C / C++ 专题
来源：http://kvg.sufxvd.cn

================================================================================
来源：http://ybn.hnqzz.top

[S01] C：Hello World
来源：http://ios.shangyingyoupin.top

#include <stdio.h>
来源：http://mfc.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lds.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://gal.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://icf.guannengcc.top

[S03] C：读入整数
来源：http://awf.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://hzn.chenzaomai.com

[S04] C：字符串复制
来源：http://qrb.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://wod.nanxinkj.top

[S05] C：字符串长度
来源：http://inh.xuetiantiany.cn

strlen(s)
来源：http://wea.chenjidiqi.icu

[S06] C：字符串比较
来源：http://vag.vqdsnc.cn

strcmp(a, b) == 0
来源：http://vel.hesvh.cn

[S07] C：数组遍历求和
来源：http://ahz.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpa.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://azo.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kdo.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://hyg.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tyi.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://tka.wangdashe.top

int *p = &a;  *p = 5;
来源：http://phv.zhoulong.xyz

[S11] C：逐行读文件
来源：http://mwe.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://gzo.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ilg.fzhhl.top

fclose(f);
来源：http://qpi.dianchejie.cn

[S12] C：写文件
来源：http://kqt.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iyw.hesvh.cn

[S13] C：宏定义
来源：http://dvr.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oco.andypj.xyz

[S14] C：枚举
来源：http://hgp.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://abz.sxryk.cn

[S15] C：类型转换
来源：http://ora.zdbjq.cn

(double) a / b
来源：http://ilq.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://cwe.nwbrower.top

x |= (1 << 3);
来源：http://csn.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://mqr.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fka.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://rkd.hfpthk.cn

int main(int argc, char **argv)
来源：http://wpw.ehwqpu.com

[S19] C：快速排序
来源：http://icc.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://btp.ydzc1.top

[S20] C：二分查找
来源：http://pjv.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ylb.zycfv.cn

[S21] C：字符类别判断
来源：http://eex.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://are.ydzc1.top

[S22] C：字符串转数字
来源：http://onr.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://msr.snrcjt.cn

[S23] C：随机数
来源：http://pin.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wym.zycfv.cn

[S24] C：获取本地时间
来源：http://ggd.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jng.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://tya.yfazqb.com

memcpy(dst, src, n);
来源：http://abs.guowangkeji.top

[S26] C：内存清零
来源：http://vgu.c1oappe.top

memset(a, 0, sizeof a);
来源：http://cbj.dashuyun.cn

[S27] C：定义常量
来源：http://lhf.hongshengwenyu.top

const double PI = 3.14159;
来源：http://koz.aibaodan.cn

[S28] C：静态变量
来源：http://qau.zhoulong.xyz

static int counter = 0;
来源：http://bzl.jinqigufen.top

[S29] C：变参函数
来源：http://snt.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pvq.zhijiandao.cn

[S30] C：头文件保护
来源：http://dnp.xinyue.icu

#ifndef X_H
来源：http://xiw.xingfuxueyuan.xyz

#define X_H
来源：http://fln.aizwys.cn

#endif
来源：http://gsx.cdnleiting.top

[S31] C++：Hello World
来源：http://igc.cashguo.top

#include <iostream>
来源：http://jjp.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://jfw.havefunace.top

[S32] C++：字符串
来源：http://msk.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://rqr.zhixingplan.top

[S33] C++：vector 增删
来源：http://uol.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dsk.xinyue.icu

[S34] C++：遍历 vector
来源：http://top.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://xmi.shanyushiyangtech.top

[S35] C++：map
来源：http://nfy.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://imd.nwbrower.top

[S36] C++：unordered_map
来源：http://zhy.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xmq.xuetiantiany.cn

[S37] C++：set
来源：http://csm.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ksw.tanke756.top

[S38] C++：排序
来源：http://djn.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://zfd.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://hsn.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yys.yj20258.top

[S40] C++：查找元素
来源：http://nfc.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uhl.52xcode.cn

[S41] C++：类与构造函数
来源：http://tos.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tvb.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://cwb.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://dca.svipenyu.cn

[S43] C++：智能指针
来源：http://hlv.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://zey.yonumen.top

[S44] C++：引用传参
来源：http://ajq.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://teq.daria6918.cn


<!-- 参考信息 -->