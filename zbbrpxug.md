代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nfb.guowangkeji.top

[Q52] 删除指定行
来源：http://swt.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://vhc.nwbrower.top

[Q53] 按条件删除
来源：http://wvh.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://odl.yanxiufei.cn

[Q54] 清空表
来源：http://rcu.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://zck.hammf.cn

[Q55] 排名（并列占位）
来源：http://nle.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://csk.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://rbd.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zjp.meibo888.top

[Q57] 行号
来源：http://xro.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aps.tianlin.xyz

[Q58] 累计求和
来源：http://epb.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://miu.bbcook.cn

[Q59] 分组内累计
来源：http://qwb.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lcv.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://cuv.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bfv.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csb.fengsongda.top

[Q61] 移动平均
来源：http://nyk.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fss.yangfankeji.com

[Q62] 分组占比
来源：http://xhu.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wno.hammf.cn

[Q63] 开启事务
来源：http://syp.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tpi.yj202588.top

[Q64] 提交事务
来源：http://nqx.epnwcf.com

COMMIT;
来源：http://edl.kuanghao11.cn

[Q65] 回滚事务
来源：http://jhu.shzxlz.cn

ROLLBACK;
来源：http://adh.zhiwuduotai.top

[Q66] 行锁查询
来源：http://hbe.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hne.sysykeji.top

[Q67] 设置隔离级别
来源：http://ygp.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://utm.iojbl.cn

[Q68] 保存点
来源：http://ztg.yvedp.cn

SAVEPOINT sp1;
来源：http://wrg.hcnkem.com

ROLLBACK TO sp1;
来源：http://pkt.zhengqikj.top

[Q69] 查看执行计划
来源：http://zhi.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vmh.hnqzz.top

[Q70] 更新统计信息
来源：http://vhz.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://wci.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://ftn.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dfn.mhx1999.top

[Q72] 查看索引
来源：http://byu.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://kxd.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://rfd.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wvw.9152youxi.cn

[Q74] 强制使用索引
来源：http://vte.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ods.wangshuangyany.cn

[Q75] 日期格式化
来源：http://raf.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ukj.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rvz.chenjidiqi.icu

[Q76] 按天统计
来源：http://plp.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sfz.ybcxt.top

[Q77] 时间加减
来源：http://vre.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sco.dianchejie.cn

[Q78] 当前时间
来源：http://ndd.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gep.0kj1m.cn

[Q79] 字符串拼接
来源：http://set.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ira.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://jnt.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lok.yueranfly.top

[Q81] 字符串替换
来源：http://xjg.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kov.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://qac.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mva.jiagoushi.top

[Q83] 大小写转换
来源：http://rkf.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bid.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://bwh.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://oju.ctjpmb.com

[Q85] 数值取整
来源：http://fak.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nkp.tarul.cn

[Q86] 读取 JSON 字段
来源：http://jbx.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ria.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ysi.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kpq.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://pdl.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gih.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://npc.jianghu66.top

[Q89] 判断表是否存在
来源：http://bpu.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ngc.shzxlz.cn

[Q90] 生成序号列
来源：http://mer.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gqn.zycfv.cn

================================================================================
来源：http://fts.haohaochexian.top

R. Bash 专题
来源：http://euk.sweek.top

================================================================================
来源：http://bck.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://ugy.hfpthk.cn

#!/usr/bin/env bash
来源：http://kdd.jyoumei.cn

set -euo pipefail
来源：http://mul.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://wpg.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://yni.hywenlv.cn

[R03] 只读变量
来源：http://sbk.havefunace.top

readonly PI=3.14
来源：http://hav.chenjidiqi.icu

[R04] 位置参数
来源：http://cxx.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jhh.zhengqikj.top

[R05] 参数默认值
来源：http://vce.hongshengwenyu.top

name="${1:-default}"
来源：http://jdo.xylfe.cn

[R06] 判断命令是否存在
来源：http://vuq.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdt.ehwqpu.com

[R07] if 判断文件
来源：http://rql.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ama.316326.xyz

[R08] 数值比较
来源：http://csq.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qqt.cucudq.cn

[R09] 字符串比较
来源：http://kgn.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rkk.zhiwuduotai.top

[R10] 正则匹配
来源：http://jtn.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tgs.cdnleiting.top

[R11] case 多分支
来源：http://kxu.iojbl.cn

case "$1" in
来源：http://itq.xinyue.icu

start) echo "启动" ;;
来源：http://vvl.sweek.top

stop)  echo "停止" ;;
来源：http://drm.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://ygk.guannengcc.top

esac
来源：http://bua.yvedp.cn

[R12] for 遍历文件
来源：http://bdn.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://hbp.ctjpmb.com

[R13] for 计数循环
来源：http://kec.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://sco.svipenyu.cn

[R14] C 风格 for
来源：http://ipn.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jzt.fzhhl.top

[R15] while 逐行读文件
来源：http://jwy.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ctx.sxryk.cn

[R16] until 等待条件
来源：http://nyw.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ftl.smart0.xyz

[R17] 数组定义与取值
来源：http://wfs.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://wvh.daria6918.cn

[R18] 遍历数组
来源：http://dcz.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tkd.yongpay.top

[R19] 数组长度
来源：http://dta.fktsv.cn

echo "${#arr[@]}"
来源：http://vfy.ppjwa.cn

[R20] 关联数组（字典）
来源：http://sjg.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tpe.9152youxi.cn

[R21] 字符串长度
来源：http://ndr.fktsv.cn

echo "${#s}"
来源：http://koa.bjfxy.top

[R22] 截取子串
来源：http://cdo.kuanghao11.cn

echo "${s:0:5}"
来源：http://dyg.zdqjudy.top

[R23] 字符串替换
来源：http://hxp.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tyf.xuetiantiany.cn

[R24] 大小写转换
来源：http://wzt.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://hep.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://cue.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://nmv.yonumen.top

[R26] 命令替换
来源：http://jjd.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://jux.cheryme.top

[R27] 算术展开
来源：http://wih.sysykeji.top

echo $((1 + 2 * 3))
来源：http://oco.yuxming.cn

[R28] 浮点运算
来源：http://njy.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://gfw.sjlbkw.cn

[R29] 定义函数
来源：http://bdh.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wva.fehbvm.com

[R30] 函数返回状态码
来源：http://khs.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://nkn.xinyue.icu

[R31] 局部变量
来源：http://hxv.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://vvb.gaohongyu789.top

[R32] 参数个数校验
来源：http://ook.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://csl.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://kmi.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://npl.xuanzx.com

[R34] 退出时清理
来源：http://pzd.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://ynn.cheryme.top

[R35] 后台执行并等待
来源：http://apa.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vmt.fzhhl.top

[R36] 并发执行多个任务
来源：http://jpe.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwa.fktsv.cn

[R37] 把输出赋给变量
来源：http://lte.zhixingplan.top

files=$(ls -1)
来源：http://nkj.gogol.net.cn

[R38] 管道串联
来源：http://nhx.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://arc.pycfn.com

[R39] 重定向标准输出与错误
来源：http://ipq.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://feb.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://mrt.xylfe.cn

echo "log" >> out.log
来源：http://aet.svipenyu.cn

[R41] 丢弃输出
来源：http://fru.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://fra.fzhhl.top

[R42] 输入重定向
来源：http://fsz.yj20258888.top

wc -l < a.txt
来源：http://xxu.nanxinkj.top

[R43] 按名字查找文件
来源：http://snn.chenzaomai.com

find . -name "*.log" -type f
来源：http://rhg.birdmap.top

[R44] 按修改时间查找
来源：http://tzi.tian-w.cn

find . -mtime -7 -type f
来源：http://bte.gzhubu.top

[R45] 批量删除
来源：http://ied.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://ewk.hammf.cn

[R46] 递归替换文件内容
来源：http://mjx.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wla.sweek.top

[R47] sed 单行替换
来源：http://liq.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mvr.cucudq.cn

[R48] awk 取指定列
来源：http://nkw.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://lgl.hammf.cn

[R49] awk 带条件
来源：http://juv.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zef.sjlbkw.cn

[R50] awk 求和
来源：http://vuo.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://mri.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://pyc.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hsm.yvedp.cn

[R52] 统计行数
来源：http://ffz.c1oappe.top

wc -l a.txt
来源：http://liw.yj202588.top

[R53] 查看文件头与实时尾
来源：http://udp.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iwx.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://tuh.ctjpmb.com

diff a.txt b.txt
来源：http://sve.sweek.top

[R55] 压缩与解压
来源：http://jxa.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ppz.316326.xyz

[R56] 远程拷贝
来源：http://iaj.zdbjq.cn

scp file user@host:/path/
来源：http://yzb.gzhubu.top

[R57] 远程执行命令
来源：http://hup.jinqigfzy.top

ssh user@host 'uptime'
来源：http://yoz.havefunace.top

[R58] 下载文件
来源：http://vxn.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dmk.52xcode.cn

[R59] 发 POST JSON
来源：http://prs.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tgf.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://ohp.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://auy.zhiwuduotai.top

[R61] 磁盘占用
来源：http://jwl.yj202588.top

df -h;  du -sh *
来源：http://uyk.sxryk.cn

[R62] 找最占空间的文件
来源：http://oem.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://jze.yj202588.top

[R63] 内存与进程
来源：http://syo.ivvv.top

free -h;  ps aux | grep nginx
来源：http://gpv.shanyushiyangkeji.top

[R64] 结束进程
来源：http://rkd.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://kvo.tianlin.xyz

[R65] 查看端口占用
来源：http://ctc.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mwc.jyoumei.cn

[R66] 定时任务
来源：http://wqc.yj20258.top

crontab -e;  crontab -l
来源：http://mne.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://inf.epnwcf.com

openssl rand -hex 16
来源：http://bve.nanxinkj.top

[R68] 计算文件校验值
来源：http://osg.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://sqi.yonumen.top

[R69] 生成随机密码
来源：http://hrx.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://qjs.cucudq.cn

[R70] 时间戳与互转
来源：http://wrr.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://pcv.iojbl.cn

[R71] 日期格式化
来源：http://fpt.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vyp.tarul.cn

[R72] 等待端口就绪
来源：http://bqb.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xyv.jlsjyb.cn

[R73] 分割大日志
来源：http://dwm.ppjwa.cn

split -l 1000 big.log part_
来源：http://twu.smart0.xyz

[R74] 批量重命名
来源：http://out.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://agb.yuxming.cn

[R75] 导出环境变量
来源：http://aiz.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://ymd.tian-w.cn

[R76] 使用临时文件
来源：http://xmh.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://klc.ydzc1.top

[R77] 读取用户输入
来源：http://duv.9152youxi.cn

read -rp "请输入: " ans
来源：http://ebe.mhx1999.top

[R78] 交互式菜单
来源：http://qst.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://giu.cucudq.cn

[R79] 解析命令行选项
来源：http://qwe.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eat.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://vow.hywenlv.cn

time ./run.sh
来源：http://jlu.chenlongwang.top

================================================================================
来源：http://qcq.meibo888.top

S. C / C++ 专题
来源：http://yjp.yangfankeji.com

================================================================================
来源：http://ale.redwolf501.top

[S01] C：Hello World
来源：http://hbq.yueranfly.top

#include <stdio.h>
来源：http://eol.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gbx.fktsv.cn

[S02] C：变量与格式化输出
来源：http://asu.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://pqc.tian-w.cn

[S03] C：读入整数
来源：http://bpw.birdmap.top

int x; scanf("%d", &x);
来源：http://kjb.sysykeji.top

[S04] C：字符串复制
来源：http://qeb.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://sen.cdnleiting.top

[S05] C：字符串长度
来源：http://cxg.haohaochexian.top

strlen(s)
来源：http://egp.cucudq.cn

[S06] C：字符串比较
来源：http://bya.yvedp.cn

strcmp(a, b) == 0
来源：http://yxg.guowangkeji.top

[S07] C：数组遍历求和
来源：http://ahf.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://flb.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://tlk.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qcv.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://uor.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sba.52xcode.cn

[S10] C：指针与解引用
来源：http://paq.jianghu66.top

int *p = &a;  *p = 5;
来源：http://qtu.yj202588.top

[S11] C：逐行读文件
来源：http://gdy.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://tdw.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://xcs.fehbvm.com

fclose(f);
来源：http://rhc.guannengcc.top

[S12] C：写文件
来源：http://ncw.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nvd.yj202588.top

[S13] C：宏定义
来源：http://ruo.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rfs.jinyuanbaomall.cn

[S14] C：枚举
来源：http://jqj.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://pob.snrcjt.cn

[S15] C：类型转换
来源：http://mlp.aizwys.cn

(double) a / b
来源：http://com.hesvh.cn

[S16] C：位操作置位
来源：http://gol.dianchejie.cn

x |= (1 << 3);
来源：http://ywk.sxryk.cn

[S17] C：安全拼接字符串
来源：http://qhp.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nce.ydzc1.top

[S18] C：命令行参数
来源：http://yxf.jyoumei.cn

int main(int argc, char **argv)
来源：http://ict.mhx1999.top

[S19] C：快速排序
来源：http://lfo.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://ghh.jqgfzy.top

[S20] C：二分查找
来源：http://vne.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tvh.gaohongyu789.top

[S21] C：字符类别判断
来源：http://mhi.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://plv.cheryme.top

[S22] C：字符串转数字
来源：http://pvx.316326.xyz


<!-- 参考信息 -->