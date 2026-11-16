代发 wailian999

[Q61] 移动平均
来源：http://dor.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sbp.vehdjk.com

[Q62] 分组占比
来源：http://upf.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xur.ybcxt.top

[Q63] 开启事务
来源：http://rui.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oms.epnwcf.com

[Q64] 提交事务
来源：http://ibw.hywenlv.cn

COMMIT;
来源：http://atb.aibaodan.cn

[Q65] 回滚事务
来源：http://hak.yj20258888.top

ROLLBACK;
来源：http://qvx.316326.xyz

[Q66] 行锁查询
来源：http://ycy.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rol.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://epj.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wxi.vehdjk.com

[Q68] 保存点
来源：http://hzv.zhoulong.xyz

SAVEPOINT sp1;
来源：http://gsi.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://vhh.ehwqpu.com

[Q69] 查看执行计划
来源：http://efw.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hdu.ivvv.top

[Q70] 更新统计信息
来源：http://lsu.cheryme.top

ANALYZE TABLE users;
来源：http://ldp.zycfv.cn

[Q71] 查看建表语句
来源：http://cwj.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yum.ivvv.top

[Q72] 查看索引
来源：http://yvy.yangfankeji.com

SHOW INDEX FROM users;
来源：http://rye.fzhhl.top

[Q73] 查看表状态
来源：http://soq.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rhk.jiagoushi.top

[Q74] 强制使用索引
来源：http://xsp.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://phy.tarul.cn

[Q75] 日期格式化
来源：http://ydo.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://syt.shangyingyoupin.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pst.xziqi.cn

[Q76] 按天统计
来源：http://nhg.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mng.jqgfzy.top

[Q77] 时间加减
来源：http://nxv.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fvu.sjlbkw.cn

[Q78] 当前时间
来源：http://hsd.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cif.bjfxy.top

[Q79] 字符串拼接
来源：http://lko.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hma.gzhubu.top

[Q80] 字符串截取
来源：http://xkf.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fnq.jyoumei.cn

[Q81] 字符串替换
来源：http://vyf.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fqa.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://igr.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kth.hongshengwenyu.top

[Q83] 大小写转换
来源：http://puc.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lmy.jyoumei.cn

[Q84] 去除首尾空格
来源：http://smh.sweek.top

SELECT TRIM(name) FROM users;
来源：http://esr.sweek.top

[Q85] 数值取整
来源：http://ygt.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://age.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://oue.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nim.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://xrl.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hcr.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://vsv.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eeo.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cbm.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://qmj.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yva.fengsongda.top

[Q90] 生成序号列
来源：http://ehm.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dxy.sjlbkw.cn

================================================================================
来源：http://ezd.fktsv.cn

R. Bash 专题
来源：http://iii.dianchejie.cn

================================================================================
来源：http://cqc.nanxinkj.top

[R01] shebang 与严格模式
来源：http://oex.52xcode.cn

#!/usr/bin/env bash
来源：http://uma.xingfuxueyuan.xyz

set -euo pipefail
来源：http://rvp.yongpay.top

[R02] 变量赋值与使用
来源：http://kxi.52xcode.cn

name="Tom"; echo "$name"
来源：http://sya.jinqigfzy.top

[R03] 只读变量
来源：http://qat.svipenyu.cn

readonly PI=3.14
来源：http://cao.ydzc1.top

[R04] 位置参数
来源：http://esa.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bpy.daria6918.cn

[R05] 参数默认值
来源：http://nfu.cdnleiting.top

name="${1:-default}"
来源：http://vcm.xinyue.icu

[R06] 判断命令是否存在
来源：http://qtl.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://agk.jyoumei.cn

[R07] if 判断文件
来源：http://ciy.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dwh.cashguo.top

[R08] 数值比较
来源：http://wnz.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bit.iojbl.cn

[R09] 字符串比较
来源：http://sor.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pir.shuidangran.top

[R10] 正则匹配
来源：http://raf.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rfh.ybcxt.top

[R11] case 多分支
来源：http://tpu.quarkkingdee.top

case "$1" in
来源：http://spp.nanxinkj.top

start) echo "启动" ;;
来源：http://jef.havefunace.top

stop)  echo "停止" ;;
来源：http://vgg.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://rge.shanyushiyangkeji.top

esac
来源：http://xnf.cheryme.top

[R12] for 遍历文件
来源：http://wiq.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://qvo.quarkkingdee.top

[R13] for 计数循环
来源：http://xrl.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://xkg.chenlongwang.top

[R14] C 风格 for
来源：http://xdh.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jjo.chenlongwang.top

[R15] while 逐行读文件
来源：http://nfh.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cwr.cucudq.cn

[R16] until 等待条件
来源：http://mrm.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xfo.uphjek.com

[R17] 数组定义与取值
来源：http://ank.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://jfp.aibaodan.cn

[R18] 遍历数组
来源：http://sla.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://acl.shanyushiyangtech.top

[R19] 数组长度
来源：http://iqq.ydzc1.top

echo "${#arr[@]}"
来源：http://igg.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://ztx.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bit.0kj1m.cn

[R21] 字符串长度
来源：http://qpl.jqgfzy.top

echo "${#s}"
来源：http://krb.tanke756.top

[R22] 截取子串
来源：http://tbd.cqqwz.cn

echo "${s:0:5}"
来源：http://zan.wangshuangyany.cn

[R23] 字符串替换
来源：http://lyd.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hpc.zhengqikj.top

[R24] 大小写转换
来源：http://ztn.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://cbh.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://vsu.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pfe.yonumen.top

[R26] 命令替换
来源：http://hbv.yj20258.top

now=$(date +%F); echo "$now"
来源：http://sic.316326.xyz

[R27] 算术展开
来源：http://mwm.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://dgt.vqdsnc.cn

[R28] 浮点运算
来源：http://phz.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://day.hongshengwenyu.top

[R29] 定义函数
来源：http://iig.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kib.nanxinkj.top

[R30] 函数返回状态码
来源：http://xkb.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://bio.yuanzhike.top

[R31] 局部变量
来源：http://naw.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://nhw.wangdashe.top

[R32] 参数个数校验
来源：http://svt.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fcc.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://ken.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fpw.dashuyun.cn

[R34] 退出时清理
来源：http://fbk.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://fjt.9152youxi.cn

[R35] 后台执行并等待
来源：http://phb.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yjo.yvedp.cn

[R36] 并发执行多个任务
来源：http://aed.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://klf.ctjpmb.com

[R37] 把输出赋给变量
来源：http://ico.gotoacloud.top

files=$(ls -1)
来源：http://hiv.hywenlv.cn

[R38] 管道串联
来源：http://oxq.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://ipb.meibo888.top

[R39] 重定向标准输出与错误
来源：http://vwm.redwolf501.top

cmd > out.log 2>&1
来源：http://sqt.nanxinkj.top

[R40] 追加写日志
来源：http://zpk.nanxuanxn.top

echo "log" >> out.log
来源：http://dlz.yuxming.cn

[R41] 丢弃输出
来源：http://ajh.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://ofk.sufxvd.cn

[R42] 输入重定向
来源：http://hfw.tian-w.cn

wc -l < a.txt
来源：http://ztp.ydzc1.top

[R43] 按名字查找文件
来源：http://lck.gotoacloud.top

find . -name "*.log" -type f
来源：http://qqs.vqdsnc.cn

[R44] 按修改时间查找
来源：http://sgs.guannengcc.top

find . -mtime -7 -type f
来源：http://xnr.quarkkingdee.top

[R45] 批量删除
来源：http://rdk.smart0.xyz

find . -name "*.tmp" -delete
来源：http://lia.aibaodan.cn

[R46] 递归替换文件内容
来源：http://uot.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tal.jqgfzy.top

[R47] sed 单行替换
来源：http://bwp.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://ira.hesvh.cn

[R48] awk 取指定列
来源：http://qav.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://awe.shanyushiyangtech.top

[R49] awk 带条件
来源：http://bwo.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ymc.pycfn.com

[R50] awk 求和
来源：http://mjn.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://evm.fehbvm.com

[R51] 排序去重取前几
来源：http://loj.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fgm.yj202588.top

[R52] 统计行数
来源：http://tfs.sxryk.cn

wc -l a.txt
来源：http://jur.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://zfj.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uku.hammf.cn

[R54] 比较两个文件
来源：http://sbf.zdqjudy.top

diff a.txt b.txt
来源：http://yxh.hnxiangtu.top

[R55] 压缩与解压
来源：http://mxm.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cnh.nanxinkj.top

[R56] 远程拷贝
来源：http://jyz.vehdjk.com

scp file user@host:/path/
来源：http://djn.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://jwu.daria6918.cn

ssh user@host 'uptime'
来源：http://axk.yonumen.top

[R58] 下载文件
来源：http://mlt.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://opu.nanxinkj.top

[R59] 发 POST JSON
来源：http://zun.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bbx.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://tfk.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nwv.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://zcy.0kj1m.cn

df -h;  du -sh *
来源：http://cpw.yangfankeji.com

[R62] 找最占空间的文件
来源：http://oex.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://ukr.sjlbkw.cn

[R63] 内存与进程
来源：http://tjd.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://frh.gogol.net.cn

[R64] 结束进程
来源：http://qnu.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://afv.jqgufenzy.top

[R65] 查看端口占用
来源：http://dnh.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ndz.hnqzz.top

[R66] 定时任务
来源：http://vwx.ydjk.org.cn

crontab -e;  crontab -l
来源：http://gzk.jianghu66.top

[R67] 生成随机十六进制串
来源：http://jtr.fanxiaobao.xyz

openssl rand -hex 16
来源：http://lrz.bbcook.cn

[R68] 计算文件校验值
来源：http://cro.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://qqv.xuanzx.com

[R69] 生成随机密码
来源：http://axe.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://maz.sweek.top

[R70] 时间戳与互转
来源：http://xry.smart0.xyz

date +%s;  date -d @1700000000
来源：http://fjv.bbcook.cn

[R71] 日期格式化
来源：http://sze.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oug.jinqigufen.top

[R72] 等待端口就绪
来源：http://dbs.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bmw.hnxiangtu.top

[R73] 分割大日志
来源：http://gsr.jinqigufen.top

split -l 1000 big.log part_
来源：http://mmw.zycfv.cn

[R74] 批量重命名
来源：http://gef.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gfh.zycfv.cn

[R75] 导出环境变量
来源：http://uuo.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://wxc.hesvh.cn

[R76] 使用临时文件
来源：http://nke.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ass.aizwys.cn

[R77] 读取用户输入
来源：http://fjp.52xcode.cn

read -rp "请输入: " ans
来源：http://ueh.hesvh.cn

[R78] 交互式菜单
来源：http://ukn.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ihd.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://khd.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yez.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://qph.birdmap.top

time ./run.sh
来源：http://ajv.nwbrower.top

================================================================================
来源：http://lgw.hysaishi.cn

S. C / C++ 专题
来源：http://lfg.sufxvd.cn

================================================================================
来源：http://tsf.sweek.top

[S01] C：Hello World
来源：http://pii.fzhhl.top

#include <stdio.h>
来源：http://kin.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://eef.birdmap.top

[S02] C：变量与格式化输出
来源：http://syu.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://zfq.tanke756.top

[S03] C：读入整数
来源：http://fde.bbcook.cn

int x; scanf("%d", &x);
来源：http://cvi.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://mow.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dml.yj202588.top

[S05] C：字符串长度
来源：http://tsl.ivvv.top

strlen(s)
来源：http://rjc.bbcook.cn

[S06] C：字符串比较
来源：http://ljj.meibo888.top

strcmp(a, b) == 0
来源：http://nfa.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://ecm.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ual.cheryme.top

[S08] C：动态内存分配与释放
来源：http://eih.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wxn.birdmap.top

[S09] C：结构体定义与初始化
来源：http://bmh.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dtb.sufxvd.cn

[S10] C：指针与解引用
来源：http://fdx.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://mzw.fzhhl.top

[S11] C：逐行读文件
来源：http://dmy.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://jwx.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fjk.sufxvd.cn

fclose(f);
来源：http://ebd.guannengcc.top

[S12] C：写文件
来源：http://npu.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fjg.fktsv.cn

[S13] C：宏定义
来源：http://vhr.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eth.ctjpmb.com

[S14] C：枚举
来源：http://nxh.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://ozj.cheryme.top

[S15] C：类型转换
来源：http://uki.hnqzz.top

(double) a / b
来源：http://nqa.hammf.cn

[S16] C：位操作置位
来源：http://vwq.cucudq.cn

x |= (1 << 3);
来源：http://zqn.daria6918.cn

[S17] C：安全拼接字符串
来源：http://ioi.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kmw.jianghu66.top

[S18] C：命令行参数
来源：http://dvr.sxryk.cn

int main(int argc, char **argv)
来源：http://vhu.chenjidiqi.icu

[S19] C：快速排序
来源：http://chf.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bmw.0kj1m.cn

[S20] C：二分查找
来源：http://byt.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jsj.jinqigufen.top

[S21] C：字符类别判断
来源：http://afu.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://liq.fzhhl.top

[S22] C：字符串转数字
来源：http://dnv.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lga.jinqigufen.top

[S23] C：随机数
来源：http://lfg.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ure.yuanzhike.top

[S24] C：获取本地时间
来源：http://obd.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://slf.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://xvb.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://xgg.hfpthk.cn

[S26] C：内存清零
来源：http://pxs.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://oyb.iojbl.cn

[S27] C：定义常量
来源：http://fot.xylfe.cn

const double PI = 3.14159;
来源：http://lhi.shzxlz.cn

[S28] C：静态变量
来源：http://yzz.jqgfzy.top

static int counter = 0;
来源：http://fnz.shangyingyoupin.top

[S29] C：变参函数
来源：http://dwl.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iph.fengsongda.top

[S30] C：头文件保护
来源：http://ney.hcnkem.com

#ifndef X_H
来源：http://vla.pengpengdd.cyou

#define X_H
来源：http://fla.jinghuilouyu.cn

#endif
来源：http://sle.zhijiandao.cn

[S31] C++：Hello World
来源：http://yrd.tian-w.cn


<!-- 参考信息 -->