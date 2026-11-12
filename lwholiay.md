代发 wailian999

SHOW INDEX FROM users;
来源：http://ayb.havefunace.top

[Q73] 查看表状态
来源：http://muc.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://nkg.nanxinkj.top

[Q74] 强制使用索引
来源：http://hfm.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vmo.jyoumei.cn

[Q75] 日期格式化
来源：http://wae.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hsn.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yul.jiagoushi.top

[Q76] 按天统计
来源：http://qmr.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jzy.yonumen.top

[Q77] 时间加减
来源：http://awy.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kpz.sysykeji.top

[Q78] 当前时间
来源：http://nff.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aep.wangdashe.top

[Q79] 字符串拼接
来源：http://dcs.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dsx.xinyue.icu

[Q80] 字符串截取
来源：http://tql.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xpm.jqgufenzy.top

[Q81] 字符串替换
来源：http://nix.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ecl.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://cas.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ozz.hesvh.cn

[Q83] 大小写转换
来源：http://iqy.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hdg.gotoacloud.top

[Q84] 去除首尾空格
来源：http://fja.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://iws.zhoulong.xyz

[Q85] 数值取整
来源：http://uaf.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hrs.yj20258.top

[Q86] 读取 JSON 字段
来源：http://zan.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pyt.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://epi.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bbs.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://bej.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wkz.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fsk.yj202588.top

[Q89] 判断表是否存在
来源：http://vms.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hjt.pycfn.com

[Q90] 生成序号列
来源：http://pwf.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cfi.aibaodan.cn

================================================================================
来源：http://rmn.andypj.xyz

R. Bash 专题
来源：http://jvx.redwolf501.top

================================================================================
来源：http://pzo.uphjek.com

[R01] shebang 与严格模式
来源：http://gvq.mhx1999.top

#!/usr/bin/env bash
来源：http://dnk.feifeiyinyue.top

set -euo pipefail
来源：http://sni.dashuyun.cn

[R02] 变量赋值与使用
来源：http://hqz.zdbjq.cn

name="Tom"; echo "$name"
来源：http://idn.wangshuangyany.cn

[R03] 只读变量
来源：http://mca.0kj1m.cn

readonly PI=3.14
来源：http://mwf.wangdashe.top

[R04] 位置参数
来源：http://ifa.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eyf.jyoumei.cn

[R05] 参数默认值
来源：http://evl.chenjidiqi.icu

name="${1:-default}"
来源：http://yvq.tianlin.xyz

[R06] 判断命令是否存在
来源：http://gve.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tmp.feifeiyinyue.top

[R07] if 判断文件
来源：http://rqp.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xad.epnwcf.com

[R08] 数值比较
来源：http://hat.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xxo.fktsv.cn

[R09] 字符串比较
来源：http://eqd.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xly.guowangkeji.top

[R10] 正则匹配
来源：http://qhb.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://csu.ydzc1.top

[R11] case 多分支
来源：http://pnj.hnxiangtu.top

case "$1" in
来源：http://pon.hysaishi.cn

start) echo "启动" ;;
来源：http://tce.jinqigufen.top

stop)  echo "停止" ;;
来源：http://wia.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://slu.zhoulong.xyz

esac
来源：http://bpx.zhijiandao.cn

[R12] for 遍历文件
来源：http://ens.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://ncd.xziqi.cn

[R13] for 计数循环
来源：http://csb.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://wlx.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://xmg.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://neb.tarul.cn

[R15] while 逐行读文件
来源：http://fee.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pyh.hongshengwenyu.top

[R16] until 等待条件
来源：http://rbc.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xcb.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://tgz.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nuy.sufxvd.cn

[R18] 遍历数组
来源：http://gic.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gwl.sjlbkw.cn

[R19] 数组长度
来源：http://mol.yuxming.cn

echo "${#arr[@]}"
来源：http://dwd.bjfxy.top

[R20] 关联数组（字典）
来源：http://gro.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mwc.jyoumei.cn

[R21] 字符串长度
来源：http://hoz.xinyue.icu

echo "${#s}"
来源：http://koi.chenzaomai.com

[R22] 截取子串
来源：http://tab.aizwys.cn

echo "${s:0:5}"
来源：http://vnd.dianchejie.cn

[R23] 字符串替换
来源：http://pmi.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://klr.ctjpmb.com

[R24] 大小写转换
来源：http://siw.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nqb.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://qso.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyw.ydjk.org.cn

[R26] 命令替换
来源：http://wyj.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://ymd.pycfn.com

[R27] 算术展开
来源：http://lkb.sweek.top

echo $((1 + 2 * 3))
来源：http://gyy.jqgfzy.top

[R28] 浮点运算
来源：http://oti.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://jmf.fzhhl.top

[R29] 定义函数
来源：http://oih.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kum.jyoumei.cn

[R30] 函数返回状态码
来源：http://iec.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://ght.hammf.cn

[R31] 局部变量
来源：http://yrw.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://ghd.gzhubu.top

[R32] 参数个数校验
来源：http://gsd.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://clj.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://ooq.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pdv.hcnkem.com

[R34] 退出时清理
来源：http://uae.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://ptj.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://uuq.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rji.snrcjt.cn

[R36] 并发执行多个任务
来源：http://esi.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iqc.bbcook.cn

[R37] 把输出赋给变量
来源：http://mxg.svipenyu.cn

files=$(ls -1)
来源：http://fhj.tian-w.cn

[R38] 管道串联
来源：http://qcw.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://trw.birdmap.top

[R39] 重定向标准输出与错误
来源：http://wfn.kuanghao11.cn

cmd > out.log 2>&1
来源：http://oqf.sufxvd.cn

[R40] 追加写日志
来源：http://fsz.wangdashe.top

echo "log" >> out.log
来源：http://owf.hongshengwenyu.top

[R41] 丢弃输出
来源：http://eta.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://ocu.daxiang520.top

[R42] 输入重定向
来源：http://fpc.gogol.net.cn

wc -l < a.txt
来源：http://lxg.ehwqpu.com

[R43] 按名字查找文件
来源：http://iky.zdqjudy.top

find . -name "*.log" -type f
来源：http://zno.jinqigfzy.top

[R44] 按修改时间查找
来源：http://lcw.9152youxi.cn

find . -mtime -7 -type f
来源：http://xsm.aibaodan.cn

[R45] 批量删除
来源：http://wcl.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://jle.meibo888.top

[R46] 递归替换文件内容
来源：http://mfr.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://owv.zhongyouzk.top

[R47] sed 单行替换
来源：http://hlv.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://lsa.zhijiandao.cn

[R48] awk 取指定列
来源：http://cfw.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://gex.0kj1m.cn

[R49] awk 带条件
来源：http://rel.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iti.hnqzz.top

[R50] awk 求和
来源：http://pur.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fig.iojbl.cn

[R51] 排序去重取前几
来源：http://mvb.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jpe.svipenyu.cn

[R52] 统计行数
来源：http://xys.nanxuanxn.top

wc -l a.txt
来源：http://idc.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://nem.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vzg.hysaishi.cn

[R54] 比较两个文件
来源：http://xvz.yonumen.top

diff a.txt b.txt
来源：http://swa.pengpengdd.cyou

[R55] 压缩与解压
来源：http://lsu.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mwi.zhixingplan.top

[R56] 远程拷贝
来源：http://pca.nanxinkj.top

scp file user@host:/path/
来源：http://uhv.xylfe.cn

[R57] 远程执行命令
来源：http://dkg.daria6918.cn

ssh user@host 'uptime'
来源：http://luo.sjlbkw.cn

[R58] 下载文件
来源：http://jxg.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dws.daxiang520.top

[R59] 发 POST JSON
来源：http://yky.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xkm.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://yuk.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hjs.52xcode.cn

[R61] 磁盘占用
来源：http://udk.chenlongwang.top

df -h;  du -sh *
来源：http://mwp.yongpay.top

[R62] 找最占空间的文件
来源：http://xtp.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://mdc.fehbvm.com

[R63] 内存与进程
来源：http://zii.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://qte.sjlbkw.cn

[R64] 结束进程
来源：http://lmy.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://lce.hongshengwenyu.top

[R65] 查看端口占用
来源：http://hpa.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dkk.daria6918.cn

[R66] 定时任务
来源：http://typ.hywenlv.cn

crontab -e;  crontab -l
来源：http://gji.cashguo.top

[R67] 生成随机十六进制串
来源：http://ojd.fktsv.cn

openssl rand -hex 16
来源：http://ovl.snrcjt.cn

[R68] 计算文件校验值
来源：http://hcb.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wyz.xylfe.cn

[R69] 生成随机密码
来源：http://unq.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://rwb.nwbrower.top

[R70] 时间戳与互转
来源：http://lvo.xinyue.icu

date +%s;  date -d @1700000000
来源：http://fak.wangshuangyany.cn

[R71] 日期格式化
来源：http://wsv.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lol.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://ihh.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://soe.fengsongda.top

[R73] 分割大日志
来源：http://phf.hesvh.cn

split -l 1000 big.log part_
来源：http://tsv.9152youxi.cn

[R74] 批量重命名
来源：http://uqw.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rdd.cqqwz.cn

[R75] 导出环境变量
来源：http://glr.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://oge.bjfxy.top

[R76] 使用临时文件
来源：http://rhv.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://idq.chenzaomai.com

[R77] 读取用户输入
来源：http://lhn.hnxiangtu.top

read -rp "请输入: " ans
来源：http://hmx.smart0.xyz

[R78] 交互式菜单
来源：http://cwt.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://dff.yj20258888.top

[R79] 解析命令行选项
来源：http://qmb.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vta.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://wjr.ppjwa.cn

time ./run.sh
来源：http://pib.hnqzz.top

================================================================================
来源：http://ymi.zhongyouzk.top

S. C / C++ 专题
来源：http://mey.gzhubu.top

================================================================================
来源：http://cjb.dianchejie.cn

[S01] C：Hello World
来源：http://uyr.vqdsnc.cn

#include <stdio.h>
来源：http://dbj.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mcv.bjfxy.top

[S02] C：变量与格式化输出
来源：http://gma.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://tnn.svipenyu.cn

[S03] C：读入整数
来源：http://iib.cdnleiting.top

int x; scanf("%d", &x);
来源：http://czt.vehdjk.com

[S04] C：字符串复制
来源：http://pjh.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ovh.xylfe.cn

[S05] C：字符串长度
来源：http://xjw.hongshengwenyu.top

strlen(s)
来源：http://bpz.tianlin.xyz

[S06] C：字符串比较
来源：http://qxo.fzhhl.top

strcmp(a, b) == 0
来源：http://tyi.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://cbu.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bnl.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://ktj.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tah.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://zye.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vfj.chenlongwang.top

[S10] C：指针与解引用
来源：http://eyh.daxiang520.top

int *p = &a;  *p = 5;
来源：http://rxo.chenzaomai.com

[S11] C：逐行读文件
来源：http://ztm.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://xlx.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mjf.hnqzz.top

fclose(f);
来源：http://uqk.xziqi.cn

[S12] C：写文件
来源：http://xvy.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqa.jqgufenzy.top

[S13] C：宏定义
来源：http://kep.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thv.yonumen.top

[S14] C：枚举
来源：http://teg.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://rwg.bjfxy.top

[S15] C：类型转换
来源：http://rqr.yj20258.top

(double) a / b
来源：http://dpx.yanxiufei.cn

[S16] C：位操作置位
来源：http://njv.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://dck.sysykeji.top

[S17] C：安全拼接字符串
来源：http://emd.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ozl.hnqzz.top

[S18] C：命令行参数
来源：http://cha.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://fym.jyoumei.cn

[S19] C：快速排序
来源：http://rtv.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iio.tarul.cn

[S20] C：二分查找
来源：http://try.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ntl.cqqwz.cn

[S21] C：字符类别判断
来源：http://eob.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://joj.iojbl.cn

[S22] C：字符串转数字
来源：http://aus.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cpq.sysykeji.top

[S23] C：随机数
来源：http://bcw.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rfp.zhongyouzk.top

[S24] C：获取本地时间
来源：http://zjo.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ips.haohaochexian.top

[S25] C：内存拷贝
来源：http://hcg.bbcook.cn

memcpy(dst, src, n);
来源：http://ajy.hnxiangtu.top

[S26] C：内存清零
来源：http://uvj.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://kfk.zhengqikj.top

[S27] C：定义常量
来源：http://rif.jlsjyb.cn

const double PI = 3.14159;
来源：http://chr.yuxming.cn

[S28] C：静态变量
来源：http://evp.sjlbkw.cn

static int counter = 0;
来源：http://lvd.ctjpmb.com

[S29] C：变参函数
来源：http://wuc.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gbe.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://rwc.svipenyu.cn

#ifndef X_H
来源：http://gry.yuanzhike.top

#define X_H
来源：http://wxu.shuidangran.top

#endif
来源：http://jjc.nanxinkj.top

[S31] C++：Hello World
来源：http://wle.iojbl.cn

#include <iostream>
来源：http://znz.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://krp.sweek.top

[S32] C++：字符串
来源：http://mge.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://yai.yfazqb.com

[S33] C++：vector 增删
来源：http://dmz.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dym.gzhubu.top

[S34] C++：遍历 vector
来源：http://kti.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://owt.dashuyun.cn

[S35] C++：map
来源：http://cys.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cmi.sjlbkw.cn

[S36] C++：unordered_map
来源：http://cbj.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fuz.shangyingyoupin.top

[S37] C++：set
来源：http://oww.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aej.chenjidiqi.icu

[S38] C++：排序
来源：http://xpn.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://cit.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://hkj.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dmt.zhijiandao.cn

[S40] C++：查找元素
来源：http://yqp.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uft.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://wov.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xmv.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://obg.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://nti.yuanzhike.top


<!-- 参考信息 -->