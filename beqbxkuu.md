代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ylv.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://zfl.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vlw.pycfn.com

[Q57] 行号
来源：http://fjy.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yba.zycfv.cn

[Q58] 累计求和
来源：http://lbu.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://whu.hammf.cn

[Q59] 分组内累计
来源：http://uvb.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nyj.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://wte.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://txf.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zqd.yonumen.top

[Q61] 移动平均
来源：http://lhd.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kep.cashguo.top

[Q62] 分组占比
来源：http://gab.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mvh.fzhhl.top

[Q63] 开启事务
来源：http://wyb.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fyu.xziqi.cn

[Q64] 提交事务
来源：http://yfd.ybcxt.top

COMMIT;
来源：http://det.yongpay.top

[Q65] 回滚事务
来源：http://fex.mhx1999.top

ROLLBACK;
来源：http://svs.jianghu66.top

[Q66] 行锁查询
来源：http://gjx.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jpu.svipenyu.cn

[Q67] 设置隔离级别
来源：http://wwy.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ief.sxryk.cn

[Q68] 保存点
来源：http://ekj.haohaochexian.top

SAVEPOINT sp1;
来源：http://puz.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://qbg.gaohongyu789.top

[Q69] 查看执行计划
来源：http://iue.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vhp.kuanghao11.cn

[Q70] 更新统计信息
来源：http://fdd.mhx1999.top

ANALYZE TABLE users;
来源：http://aff.gzhubu.top

[Q71] 查看建表语句
来源：http://usi.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://roo.dashuyun.cn

[Q72] 查看索引
来源：http://nxh.ehwqpu.com

SHOW INDEX FROM users;
来源：http://jls.316326.xyz

[Q73] 查看表状态
来源：http://tqu.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://omp.xylfe.cn

[Q74] 强制使用索引
来源：http://tlv.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kac.gotoacloud.top

[Q75] 日期格式化
来源：http://vjj.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gew.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvk.jinghuilouyu.cn

[Q76] 按天统计
来源：http://pqm.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://osd.shzxlz.cn

[Q77] 时间加减
来源：http://xvu.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hqx.feifeiyinyue.top

[Q78] 当前时间
来源：http://gzs.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pha.meibo888.top

[Q79] 字符串拼接
来源：http://ego.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jll.wangdashe.top

[Q80] 字符串截取
来源：http://pgh.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nno.sjlbkw.cn

[Q81] 字符串替换
来源：http://lfi.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xns.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://mpy.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urz.sufxvd.cn

[Q83] 大小写转换
来源：http://wwx.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uah.pycfn.com

[Q84] 去除首尾空格
来源：http://jwn.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://zjc.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://dlt.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fvg.cashguo.top

[Q86] 读取 JSON 字段
来源：http://bzy.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pkm.ydzc1.top

[Q87] JSON 字段做条件
来源：http://adi.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zbd.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://mgt.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mni.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ydc.svipenyu.cn

[Q89] 判断表是否存在
来源：http://kqg.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lgi.hnqzz.top

[Q90] 生成序号列
来源：http://bad.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rhr.kuanghao11.cn

================================================================================
来源：http://edy.hysaishi.cn

R. Bash 专题
来源：http://nrc.ywan-chungtsiang.top

================================================================================
来源：http://enq.vehdjk.com

[R01] shebang 与严格模式
来源：http://hre.vehdjk.com

#!/usr/bin/env bash
来源：http://wek.chenjidiqi.icu

set -euo pipefail
来源：http://opl.guowangkeji.top

[R02] 变量赋值与使用
来源：http://gyo.jiagoushi.top

name="Tom"; echo "$name"
来源：http://ywv.andypj.xyz

[R03] 只读变量
来源：http://wbd.guannengcc.top

readonly PI=3.14
来源：http://qnf.kuanghao11.cn

[R04] 位置参数
来源：http://bkm.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yef.zhijiandao.cn

[R05] 参数默认值
来源：http://mir.ppjwa.cn

name="${1:-default}"
来源：http://dpq.ivvv.top

[R06] 判断命令是否存在
来源：http://uzu.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kim.gogol.net.cn

[R07] if 判断文件
来源：http://whj.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dsi.shanyushiyangkeji.top

[R08] 数值比较
来源：http://rvc.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rcm.cdnleiting.top

[R09] 字符串比较
来源：http://lci.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iys.fehbvm.com

[R10] 正则匹配
来源：http://rab.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kyb.yvedp.cn

[R11] case 多分支
来源：http://jul.tianlin.xyz

case "$1" in
来源：http://zlf.52xcode.cn

start) echo "启动" ;;
来源：http://syy.gotoacloud.top

stop)  echo "停止" ;;
来源：http://gfl.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://uaw.hysaishi.cn

esac
来源：http://ash.cucudq.cn

[R12] for 遍历文件
来源：http://wdu.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://edg.daria6918.cn

[R13] for 计数循环
来源：http://dza.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ztb.yueranfly.top

[R14] C 风格 for
来源：http://yyy.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hyn.zdqjudy.top

[R15] while 逐行读文件
来源：http://sno.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://evf.redwolf501.top

[R16] until 等待条件
来源：http://cwo.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ysq.aibaodan.cn

[R17] 数组定义与取值
来源：http://axr.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ixd.ppjwa.cn

[R18] 遍历数组
来源：http://mei.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://abd.wangdashe.top

[R19] 数组长度
来源：http://tsm.vqdsnc.cn

echo "${#arr[@]}"
来源：http://tbm.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://xey.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxd.yvedp.cn

[R21] 字符串长度
来源：http://yxr.jinyuanbaomall.cn

echo "${#s}"
来源：http://inx.yanxiufei.cn

[R22] 截取子串
来源：http://tlw.zhijiandao.cn

echo "${s:0:5}"
来源：http://lhj.pengpengdd.cyou

[R23] 字符串替换
来源：http://onm.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kzn.aizwys.cn

[R24] 大小写转换
来源：http://laf.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://stp.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://kjz.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ybd.yj202588.top

[R26] 命令替换
来源：http://mrd.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://zmo.xziqi.cn

[R27] 算术展开
来源：http://piy.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://fhi.epnwcf.com

[R28] 浮点运算
来源：http://lkx.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://dvf.fanxiaobao.xyz

[R29] 定义函数
来源：http://qxi.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iav.havefunace.top

[R30] 函数返回状态码
来源：http://xwg.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://rqs.guannengcc.top

[R31] 局部变量
来源：http://ljo.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://wwn.bbcook.cn

[R32] 参数个数校验
来源：http://arp.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fpq.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://lsi.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfj.wangdashe.top

[R34] 退出时清理
来源：http://rmo.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sug.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://hli.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jax.fzhhl.top

[R36] 并发执行多个任务
来源：http://xqh.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cbm.ppjwa.cn

[R37] 把输出赋给变量
来源：http://vkt.jianghu66.top

files=$(ls -1)
来源：http://xvl.hesvh.cn

[R38] 管道串联
来源：http://qkn.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://luo.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://wjz.jqgufenzy.top

cmd > out.log 2>&1
来源：http://eel.dianchejie.cn

[R40] 追加写日志
来源：http://kla.jqgufenzy.top

echo "log" >> out.log
来源：http://opr.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://bxl.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://wwb.hfpthk.cn

[R42] 输入重定向
来源：http://ezc.sufxvd.cn

wc -l < a.txt
来源：http://dqy.hysaishi.cn

[R43] 按名字查找文件
来源：http://jrd.cheryme.top

find . -name "*.log" -type f
来源：http://guj.zhengqikj.top

[R44] 按修改时间查找
来源：http://xav.ivvv.top

find . -mtime -7 -type f
来源：http://lrw.redwolf501.top

[R45] 批量删除
来源：http://zgn.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://zzo.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://crj.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xcz.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://bvn.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://bby.zhongyouzk.top

[R48] awk 取指定列
来源：http://zvy.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://ryn.yfazqb.com

[R49] awk 带条件
来源：http://uca.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jxj.jqgfzy.top

[R50] awk 求和
来源：http://mmr.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bri.hywenlv.cn

[R51] 排序去重取前几
来源：http://pdt.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zvq.yanxiufei.cn

[R52] 统计行数
来源：http://dff.dashuyun.cn

wc -l a.txt
来源：http://mni.cheryme.top

[R53] 查看文件头与实时尾
来源：http://zsp.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fej.jinqigufen.top

[R54] 比较两个文件
来源：http://tkj.aibaodan.cn

diff a.txt b.txt
来源：http://ovg.sjlbkw.cn

[R55] 压缩与解压
来源：http://erw.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://acl.jinqigfzy.top

[R56] 远程拷贝
来源：http://pye.kuanghao11.cn

scp file user@host:/path/
来源：http://dyx.tian-w.cn

[R57] 远程执行命令
来源：http://ozk.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://cwq.yonumen.top

[R58] 下载文件
来源：http://zft.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vqb.gaohongyu789.top

[R59] 发 POST JSON
来源：http://vup.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iks.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://xhw.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zcs.sysykeji.top

[R61] 磁盘占用
来源：http://der.hammf.cn

df -h;  du -sh *
来源：http://vqm.ehwqpu.com

[R62] 找最占空间的文件
来源：http://khs.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://ppe.jyoumei.cn

[R63] 内存与进程
来源：http://kcl.meibo888.top

free -h;  ps aux | grep nginx
来源：http://smh.jinqigfzy.top

[R64] 结束进程
来源：http://jsq.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://wue.gogol.net.cn

[R65] 查看端口占用
来源：http://twa.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tqk.gaohongyu789.top

[R66] 定时任务
来源：http://zif.yj20258888.top

crontab -e;  crontab -l
来源：http://qxl.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://ygg.jinghuilouyu.cn

openssl rand -hex 16
来源：http://kql.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://hey.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cyd.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://hxn.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://zub.cucudq.cn

[R70] 时间戳与互转
来源：http://rkq.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://ntp.hesvh.cn

[R71] 日期格式化
来源：http://tnb.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pym.gzhubu.top

[R72] 等待端口就绪
来源：http://omt.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tly.hywenlv.cn

[R73] 分割大日志
来源：http://mlb.redwolf501.top

split -l 1000 big.log part_
来源：http://xmt.xuanzx.com

[R74] 批量重命名
来源：http://ens.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qpk.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://wll.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pmn.jinqigfzy.top

[R76] 使用临时文件
来源：http://ivi.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kmm.316326.xyz

[R77] 读取用户输入
来源：http://wkn.gotoacloud.top

read -rp "请输入: " ans
来源：http://geo.jyoumei.cn

[R78] 交互式菜单
来源：http://hli.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ydy.jyoumei.cn

[R79] 解析命令行选项
来源：http://gep.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wkh.hcnkem.com

[R80] 查看脚本执行耗时
来源：http://sdm.jiagoushi.top

time ./run.sh
来源：http://qtv.nwbrower.top

================================================================================
来源：http://fnw.jyoumei.cn

S. C / C++ 专题
来源：http://pyc.dashuyun.cn

================================================================================
来源：http://rfn.svipenyu.cn

[S01] C：Hello World
来源：http://hcb.sysykeji.top

#include <stdio.h>
来源：http://faf.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://abd.pycfn.com

[S02] C：变量与格式化输出
来源：http://iwa.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://zrl.zhijiandao.cn

[S03] C：读入整数
来源：http://dhq.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://crf.zhengqikj.top

[S04] C：字符串复制
来源：http://mbs.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://jdt.dashuyun.cn

[S05] C：字符串长度
来源：http://xnv.feifeiyinyue.top

strlen(s)
来源：http://ynb.ppjwa.cn

[S06] C：字符串比较
来源：http://mol.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://sqc.316326.xyz

[S07] C：数组遍历求和
来源：http://xya.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vlg.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://cem.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nch.shuidangran.top

[S09] C：结构体定义与初始化
来源：http://bwt.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypm.bbcook.cn

[S10] C：指针与解引用
来源：http://bnz.cheryme.top

int *p = &a;  *p = 5;
来源：http://cvc.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://pef.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://nop.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lbo.aizwys.cn

fclose(f);
来源：http://gsx.ydzc1.top

[S12] C：写文件
来源：http://que.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cet.meibo888.top

[S13] C：宏定义
来源：http://cfz.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lgz.shangyingyoupin.top

[S14] C：枚举
来源：http://bei.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ggk.sufxvd.cn

[S15] C：类型转换
来源：http://nye.jyoumei.cn

(double) a / b
来源：http://uxb.tian-w.cn

[S16] C：位操作置位
来源：http://ivi.zhixingplan.top

x |= (1 << 3);
来源：http://ujc.tarul.cn

[S17] C：安全拼接字符串
来源：http://jbp.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnp.zhongyouzk.top

[S18] C：命令行参数
来源：http://czk.dianchejie.cn

int main(int argc, char **argv)
来源：http://olc.wangdashe.top

[S19] C：快速排序
来源：http://ick.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://mkl.andypj.xyz

[S20] C：二分查找
来源：http://xlx.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hsa.gaohongyu789.top

[S21] C：字符类别判断
来源：http://tht.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vqd.fengsongda.top

[S22] C：字符串转数字
来源：http://bxo.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://dab.zhongyouzk.top

[S23] C：随机数
来源：http://ryy.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gby.zhixingplan.top

[S24] C：获取本地时间
来源：http://ldm.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ngs.ppjwa.cn

[S25] C：内存拷贝
来源：http://hud.jianghu66.top

memcpy(dst, src, n);
来源：http://lxd.wangdashe.top

[S26] C：内存清零
来源：http://gzu.sysykeji.top


<!-- 参考信息 -->