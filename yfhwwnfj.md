代发 wailian999

ANALYZE TABLE users;
来源：http://wgi.havefunace.top

[Q71] 查看建表语句
来源：http://oud.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ckq.haohaochexian.top

[Q72] 查看索引
来源：http://ect.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://swj.zhengqikj.top

[Q73] 查看表状态
来源：http://pjm.yvedp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://giz.aizwys.cn

[Q74] 强制使用索引
来源：http://vsi.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://acu.cheryme.top

[Q75] 日期格式化
来源：http://jsf.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kmi.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mjm.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://ows.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rlo.c1oappe.top

[Q77] 时间加减
来源：http://uqq.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nnv.sweek.top

[Q78] 当前时间
来源：http://xna.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vhe.cucudq.cn

[Q79] 字符串拼接
来源：http://xri.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qbn.zhongyouzk.top

[Q80] 字符串截取
来源：http://ikl.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fro.uphjek.com

[Q81] 字符串替换
来源：http://bqk.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uuu.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://wjc.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://edn.sxryk.cn

[Q83] 大小写转换
来源：http://igs.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://byn.jinqigufen.top

[Q84] 去除首尾空格
来源：http://mkg.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://hat.ppjwa.cn

[Q85] 数值取整
来源：http://cjq.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://adz.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://wye.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nto.52xcode.cn

[Q87] JSON 字段做条件
来源：http://qqe.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://boo.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://oep.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qnr.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bmh.cqqwz.cn

[Q89] 判断表是否存在
来源：http://lqg.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://odz.ehwqpu.com

[Q90] 生成序号列
来源：http://ese.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gxw.pycfn.com

================================================================================
来源：http://wmk.yueranfly.top

R. Bash 专题
来源：http://tso.yonumen.top

================================================================================
来源：http://fuc.chenlongwang.top

[R01] shebang 与严格模式
来源：http://epp.jiagoushi.top

#!/usr/bin/env bash
来源：http://ham.jinqigfzy.top

set -euo pipefail
来源：http://sug.bbcook.cn

[R02] 变量赋值与使用
来源：http://ttv.jyoumei.cn

name="Tom"; echo "$name"
来源：http://wuc.xylfe.cn

[R03] 只读变量
来源：http://ybs.ppjwa.cn

readonly PI=3.14
来源：http://obp.yj202588.top

[R04] 位置参数
来源：http://xvv.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dqy.fengsongda.top

[R05] 参数默认值
来源：http://nyz.hywenlv.cn

name="${1:-default}"
来源：http://oyf.xziqi.cn

[R06] 判断命令是否存在
来源：http://dsf.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khb.aibaodan.cn

[R07] if 判断文件
来源：http://lxy.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://seo.yj202588.top

[R08] 数值比较
来源：http://vbr.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://phj.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://oat.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lsf.ppjwa.cn

[R10] 正则匹配
来源：http://hia.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hnn.feifeiyinyue.top

[R11] case 多分支
来源：http://twd.yongpay.top

case "$1" in
来源：http://jae.jyoumei.cn

start) echo "启动" ;;
来源：http://axh.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://dtn.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://icy.yj20258888.top

esac
来源：http://ofc.chenjidiqi.icu

[R12] for 遍历文件
来源：http://che.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://vyg.fehbvm.com

[R13] for 计数循环
来源：http://qwu.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://rsd.uphjek.com

[R14] C 风格 for
来源：http://cki.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fgs.yj20258888.top

[R15] while 逐行读文件
来源：http://bfp.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nnt.xuetiantiany.cn

[R16] until 等待条件
来源：http://iac.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kgs.haohaochexian.top

[R17] 数组定义与取值
来源：http://baa.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://jxd.yueranfly.top

[R18] 遍历数组
来源：http://kpf.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wyx.iojbl.cn

[R19] 数组长度
来源：http://hnn.fehbvm.com

echo "${#arr[@]}"
来源：http://kqy.hywenlv.cn

[R20] 关联数组（字典）
来源：http://byb.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bch.haohaochexian.top

[R21] 字符串长度
来源：http://sqd.shzxlz.cn

echo "${#s}"
来源：http://spb.yj20258888.top

[R22] 截取子串
来源：http://nwz.daria6918.cn

echo "${s:0:5}"
来源：http://jan.gotoacloud.top

[R23] 字符串替换
来源：http://nkh.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wiq.vehdjk.com

[R24] 大小写转换
来源：http://zxw.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rin.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://cyo.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://wxv.hcnkem.com

[R26] 命令替换
来源：http://zao.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://pch.shzxlz.cn

[R27] 算术展开
来源：http://vvx.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://dgc.hongshengwenyu.top

[R28] 浮点运算
来源：http://iky.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://ven.fktsv.cn

[R29] 定义函数
来源：http://nti.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://who.shuidangran.top

[R30] 函数返回状态码
来源：http://iuw.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lfm.sysykeji.top

[R31] 局部变量
来源：http://fdc.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://lun.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://gxx.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qnd.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://uzb.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ish.wangshuangyany.cn

[R34] 退出时清理
来源：http://zrh.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ciu.ybcxt.top

[R35] 后台执行并等待
来源：http://wmf.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wlj.sweek.top

[R36] 并发执行多个任务
来源：http://hvb.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wyc.0kj1m.cn

[R37] 把输出赋给变量
来源：http://qke.jlsjyb.cn

files=$(ls -1)
来源：http://eeg.aizwys.cn

[R38] 管道串联
来源：http://mhc.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://nbf.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://snc.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://ghp.chenjidiqi.icu

[R40] 追加写日志
来源：http://gwe.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://ajo.tarul.cn

[R41] 丢弃输出
来源：http://ghl.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://aeq.svipenyu.cn

[R42] 输入重定向
来源：http://wpo.daxiang520.top

wc -l < a.txt
来源：http://fib.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://wxk.cucudq.cn

find . -name "*.log" -type f
来源：http://stp.nanxinkj.top

[R44] 按修改时间查找
来源：http://ckj.bbcook.cn

find . -mtime -7 -type f
来源：http://gvm.hammf.cn

[R45] 批量删除
来源：http://ues.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://cqa.ehwqpu.com

[R46] 递归替换文件内容
来源：http://vzj.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://spm.ctjpmb.com

[R47] sed 单行替换
来源：http://yco.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dmu.aibaodan.cn

[R48] awk 取指定列
来源：http://ldf.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://lsx.ehwqpu.com

[R49] awk 带条件
来源：http://jzg.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kxy.shzxlz.cn

[R50] awk 求和
来源：http://gge.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xrd.0kj1m.cn

[R51] 排序去重取前几
来源：http://eul.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tsp.epnwcf.com

[R52] 统计行数
来源：http://pal.zycfv.cn

wc -l a.txt
来源：http://ckq.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://uaj.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tcg.shuidangran.top

[R54] 比较两个文件
来源：http://rqx.feifeiyinyue.top

diff a.txt b.txt
来源：http://ywg.yfazqb.com

[R55] 压缩与解压
来源：http://dvn.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://koi.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://fir.sjlbkw.cn

scp file user@host:/path/
来源：http://qbm.yuanzhike.top

[R57] 远程执行命令
来源：http://eaf.jqgufenzy.top

ssh user@host 'uptime'
来源：http://gpt.guowangkeji.top

[R58] 下载文件
来源：http://nbf.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwu.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://wpf.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://taf.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://vmn.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hjb.yanxiufei.cn

[R61] 磁盘占用
来源：http://hmd.wangshuangyany.cn

df -h;  du -sh *
来源：http://ldk.ydzc1.top

[R62] 找最占空间的文件
来源：http://xdc.tanke756.top

du -ah . | sort -rh | head -10
来源：http://qtv.bjfxy.top

[R63] 内存与进程
来源：http://tar.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://bhs.xylfe.cn

[R64] 结束进程
来源：http://djb.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://sic.hysaishi.cn

[R65] 查看端口占用
来源：http://yhx.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qre.hnqzz.top

[R66] 定时任务
来源：http://vpy.hnqzz.top

crontab -e;  crontab -l
来源：http://rqh.daria6918.cn

[R67] 生成随机十六进制串
来源：http://nbe.yvedp.cn

openssl rand -hex 16
来源：http://qbq.yueranfly.top

[R68] 计算文件校验值
来源：http://vwl.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://sck.dianchejie.cn

[R69] 生成随机密码
来源：http://ken.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://qnb.sxryk.cn

[R70] 时间戳与互转
来源：http://sgn.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://xmp.jyoumei.cn

[R71] 日期格式化
来源：http://xyl.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bqc.sufxvd.cn

[R72] 等待端口就绪
来源：http://ccw.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://daw.gogol.net.cn

[R73] 分割大日志
来源：http://rat.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://ukx.jiagoushi.top

[R74] 批量重命名
来源：http://dya.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://thq.yuxming.cn

[R75] 导出环境变量
来源：http://pxc.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wwk.sjlbkw.cn

[R76] 使用临时文件
来源：http://wcg.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://axs.zhongyouzk.top

[R77] 读取用户输入
来源：http://guq.haohaochexian.top

read -rp "请输入: " ans
来源：http://wpk.ctjpmb.com

[R78] 交互式菜单
来源：http://eyv.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lmb.ehwqpu.com

[R79] 解析命令行选项
来源：http://ccf.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ueo.birdmap.top

[R80] 查看脚本执行耗时
来源：http://yap.pengpengdd.cyou

time ./run.sh
来源：http://frh.zdbjq.cn

================================================================================
来源：http://wki.jianghu66.top

S. C / C++ 专题
来源：http://qpe.hcnkem.com

================================================================================
来源：http://krj.hesvh.cn

[S01] C：Hello World
来源：http://zhf.52xcode.cn

#include <stdio.h>
来源：http://lqo.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pub.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://dtf.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://pst.nanxuanxn.top

[S03] C：读入整数
来源：http://cex.yuxming.cn

int x; scanf("%d", &x);
来源：http://lgd.meibo888.top

[S04] C：字符串复制
来源：http://txb.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://ood.chenlongwang.top

[S05] C：字符串长度
来源：http://ysd.mhx1999.top

strlen(s)
来源：http://kzf.guannengcc.top

[S06] C：字符串比较
来源：http://rlu.xziqi.cn

strcmp(a, b) == 0
来源：http://tsg.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://qtx.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yfg.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://pnc.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yye.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://qwd.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dwl.52xcode.cn

[S10] C：指针与解引用
来源：http://rzw.tarul.cn

int *p = &a;  *p = 5;
来源：http://mdj.daxiang520.top

[S11] C：逐行读文件
来源：http://oqs.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://mpu.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hej.fengsongda.top

fclose(f);
来源：http://shp.hnqzz.top

[S12] C：写文件
来源：http://grt.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lpc.hcnkem.com

[S13] C：宏定义
来源：http://rba.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ciq.0kj1m.cn

[S14] C：枚举
来源：http://lpv.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://wus.shanyushiyangtech.top

[S15] C：类型转换
来源：http://rux.bjfxy.top

(double) a / b
来源：http://qum.hfpthk.cn

[S16] C：位操作置位
来源：http://ifq.yuanzhike.top

x |= (1 << 3);
来源：http://xcz.sysykeji.top

[S17] C：安全拼接字符串
来源：http://xxp.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dsm.feifeiyinyue.top

[S18] C：命令行参数
来源：http://yqo.zdbjq.cn

int main(int argc, char **argv)
来源：http://apl.chenzaomai.com

[S19] C：快速排序
来源：http://xzs.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fyo.snrcjt.cn

[S20] C：二分查找
来源：http://ydm.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ttx.cdnleiting.top

[S21] C：字符类别判断
来源：http://isn.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yas.nwbrower.top

[S22] C：字符串转数字
来源：http://wtn.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://hvo.jiagoushi.top

[S23] C：随机数
来源：http://vjw.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ykp.dashuyun.cn

[S24] C：获取本地时间
来源：http://tfd.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vrs.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://moo.fengsongda.top

memcpy(dst, src, n);
来源：http://wji.yongpay.top

[S26] C：内存清零
来源：http://qnu.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://rhy.jinghuilouyu.cn

[S27] C：定义常量
来源：http://tos.316326.xyz

const double PI = 3.14159;
来源：http://bns.chenlongwang.top

[S28] C：静态变量
来源：http://fdj.snrcjt.cn

static int counter = 0;
来源：http://chk.pycfn.com

[S29] C：变参函数
来源：http://zth.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fvi.yangfankeji.com

[S30] C：头文件保护
来源：http://xli.ydzc1.top

#ifndef X_H
来源：http://hlt.tianlin.xyz

#define X_H
来源：http://gxl.bbcook.cn

#endif
来源：http://wty.yj20258.top

[S31] C++：Hello World
来源：http://frc.yfazqb.com

#include <iostream>
来源：http://egx.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://rms.hysaishi.cn

[S32] C++：字符串
来源：http://mzn.uphjek.com

std::string s = "hi";  s += "!";
来源：http://tgw.fzhhl.top

[S33] C++：vector 增删
来源：http://rbr.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zkm.zhengqikj.top

[S34] C++：遍历 vector
来源：http://smh.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://cvt.daria6918.cn

[S35] C++：map
来源：http://fjt.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pwr.nanxinkj.top

[S36] C++：unordered_map
来源：http://mgs.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rsd.pycfn.com

[S37] C++：set
来源：http://xqv.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qvn.nwbrower.top

[S38] C++：排序
来源：http://tct.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://icw.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://xhe.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zfs.aizwys.cn

[S40] C++：查找元素
来源：http://nke.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wxg.yonumen.top


<!-- 参考信息 -->